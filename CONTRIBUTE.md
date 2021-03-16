
# How to Contribute Guide

First of all, register yourself in [this form](https://forms.gle/P2Kwuqew94FosvWq5). We will add you to the #trusted-setup-phase2-ceremony channel in the Hermez Discord.

You can also reach us in the [Hermez Telegram group](https://t.me/hermez_network).

## Requirements

A machine with 4 cores and 16Gb would do the work, but we recommend a bigger machine to process the ceremony faster.

In this tutorial I'll describe all the steps required to run them in a new m5a.4xlarge AWS instance with ubuntu 20.04. The actual cost of this instance at the moment of writing is 0.644$/h  But this is just for reference. Actually, it's better if you run your own hardware.

You can use any machine to run the ceremony. The important part of the ceremony is that the toxic value is not leaked and it's deleted after the completion of the ceremony.

This toxic value is in the memory while the ceremony is running. This toxic value is not displayed anywhere and it's not stored anywhere. It's recomended to restart the machine after the ceremony is completed to be sure this toxic value is not accessible any more.

You can check the [Phase1 Perpetual Powers of Tau Ceremony](https://github.com/weijiekoh/perpetualpowersoftau) used by Hermez for geting ideas of what to do to be sure the toxic value is deleted.

## Preparation of the Machine.

You will need node version at least v14. For reference we are using v14.8.0

Quick instructions to install node if you don't have it:

````
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.2/install.sh | bash
source ~/.bashrc
nvm install v14.8.0
node --version
````

Install snarkjs:

````bash
npm install -g snarkjs
````

At the begining of the contribution you will receive 3 files:

* `circuit-1912-32-256-64_hez3_xxxx.zkey` (60GB)
* `circuit-344-32-256-64_hez3_xxxx.zkey`  (15GB)
* `withdraw_hez3_xxxx.zkey` (50MB)

Where `xxxx` is the contribution of the last participant.

````
wget --compression=none https://hermez.s3-eu-west-1.amazonaws.com/withdraw_hez3_xxxx.zkey
wget --compression=none https://hermez.s3-eu-west-1.amazonaws.com/circuit-344-32-256-64_hez3_xxxx.zkey
wget --compression=none https://hermez.s3-eu-west-1.amazonaws.com/circuit-1912-32-256-64_hez3_xxxx.zkey
````

Take note of the blake2b of the inputs and check with the ceremony coordinator the integrity of the files:
````bash
b2sum circuit-1912-32-256-64_hez3_xxxx.zkey
b2sum circuit-344-32-256-64_hez3_xxxx.zkey
b2sum withdraw_hez3_xxxx.zkey
````

To run the ceremony you need to run:

````bash
snarkjs zkey contribute circuit-1912-32-256-64_hez3_xxxx.zkey circuit-1912-32-256-64_hez3_yyyy.zkey -v -n=yourName
````

Substitute `yourName` for the name you want to appear in the file. Please do not uses spaces or special characters so we don't have problems.  This name is important because this is what will be displayed, together with the contribution hash when all the contributions are listed in the final zkey file verification.

Substitute also `yyyy` by the actual contrubution.  This should be `xxxx` + 1.

Write down the Circuit Hash and The Contribution Hash printed at the end.

The circuit hash for the 1912Txs circuit should be:

````
07b5cfaa d2d4674e 095f20dd 11e516bc
e8aa1d3e 59174e10 e538504d 208bc959
5c05e470 3db00d49 212258a3 12da9230
83a819ea 56af7132 e12996f3 13882859
````

This Hash is computed at the phase two preparation, and depends on the r1cs file and the Powers of Tau result ceremony.

Do the same for the other two circuits:

````bash
snarkjs zkey contribute circuit-344-32-256-64_hez3_xxxx.zkey circuit-344-32-256-64_hez3_yyyy.zkey -v -n=yourName
snarkjs zkey contribute withdraw_hez3_xxxx.zkey withdraw_hez3_yyyy.zkey -v -n=yourName
````

The circuit hash for `circuit-344-32-256-64` should be:

````
b6b78d08 04636911 0d12afad 8c49a0e9
5c0b03ed 99f2ff8e dedf2d51 dd427750
2a9ca1b7 5417069e 174ce637 da105132
ea8b5448 21ca6ade 4df911cd 52d34550
````

And the circuit hash of the `withdraw` circuit should be:

````
26f8883b 44e999e7 dc749bac d7a914e3
4fe4602e bb18d681 39a70cd9 16c22722
2ec186f5 1dd876d1 04a403df 13433b27
7c0c69a3 3a2aca64 dc3365c0 ce74a0ec
````

Write down the contribution hash for both circuits.

Now you can compute the checksum of your contribution results.

````bash
b2sum circuit-1912-32-256-64_hez3_yyyy.zkey
b2sum circuit-344-32-256-64_hez3_yyyy.zkey
b2sum withdraw_hez3_yyyy.zkey
````

With this, you will have all the information to fill the attestation template.

Create a copy of the [template_attestation.md](template_attestation.md) with name `yyyy_yourName_attestation.txt`

Fill all the fields of the template.

Sign the template with a PGP key or Keybase.

And generate a signed attestation with name:
`yyyy_yourName_attestation_signed.txt`


Send the 3 responses plus the signed attestation to the coordinator.

You will be asked to do so by first creating a ssh-key if you don't have it.

````bash
ssh-keygen -t rsa -q -f "$HOME/.ssh/id_rsa" -N ""
````

Send the public key to the ceremony coordinator.
You can see your public key by typing:

````bash
cat ~/.ssh/id_rsa.pub
````

Once the ceremony coordinator authorizes your key, you can upload the generated files and the signed attestation by doing:

````bash
sftp contributor_yyyy@s-628cadcefdfd40e39.server.transfer.us-east-1.amazonaws.com <<< $'put circuit-1912-32-256-64_hez3_yyyy.zkey'
sftp contributor_yyyy@s-628cadcefdfd40e39.server.transfer.us-east-1.amazonaws.com <<< $'put circuit-344-32-256-64_hez3_yyyy.zkey'
sftp contributor_yyyy@s-628cadcefdfd40e39.server.transfer.us-east-1.amazonaws.com <<< $'put withdraw_hez3_yyyy.zkey'
sftp contributor_yyyy@s-628cadcefdfd40e39.server.transfer.us-east-1.amazonaws.com <<< $'put yyyy_YourName_attestation_signed.txt'
````

Send also your public PGP Key or a link to yout PGP keybase to the coordinator.

Thank you very much for contributing!
