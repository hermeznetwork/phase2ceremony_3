# Hermez First Phase 2 ceremony attestation

**Contribution Number:** 0006

**Name:** Koh Wei Jie

**Date:** March 18 - 19 2021

**Location:** The cloud

**Device:** Google Cloud VM n2d-standard-8 (2 vCPUs, 8 GB memory)
Confidential VM service enabled

I used a Google Cloud account enrolled in [Google's Advanced Protection
Program](https://landing.google.com/advancedprotection/). The Confidential
Computing option purports to provide encryption to data in the cloud while it
is being processed. I can't speak to whether this service is truly secure, but
generally, the more diverse the hardware/VMs used, the more secure the
ceremony. As such, even if Confidential Computing is only as secure than a
regular Google Cloud VM, an adversary will have the already difficult task of
compromising Google Cloud in addition to compromising every other participant's
device.

**Entropy sources:** Hex values from [the Australian
National University's Quantum Random Number
Generator](https://qrng.anu.edu.au/random-hex/) and the output of `python3 -c
'import secrets; print(secrets.token_hex(40960))'` from my laptop.

I downloaded the following files and checked that their Blake2 hashes match
those attested by the previous participant.

```
075f7167252fa63f8ae98727c979aa4ea7a0648e05be0bbcb92253a5470ebc766442107059fae2b1686ff7eefba2a1b6192bc72808b55c5eaa14b168d6f95db9  circuit-1912-32-256-64_hez3_0005.zkey
032d8e6da8cbd7c2f3ab5be4cb86fd6bf191630f13429d0775cd2e732093a6230037a4b2438d45c22b7cec7de9147fa7d06e9bbe727961abc58e7c3c9737c48a  circuit-344-32-256-64_hez3_0005.zkey
a6dc6c1367b3c5e8da80a2062c0c0aaef408fd9578d3bb2d5eb644a27542debd9fd2f1b569cefc7f7ac84439873b7f53fb3072ae544adb8e1dcf217195d14a04  withdraw_hez3_0005.zkey
```

## My contributions

The Blake2 checksums of my contribution files are:

```
fc64929f7d30899d763cac628b643764525f09c4607d60a696a9465837847c9d5abd8683734ef843c8cdffd898a85ce3b3b576946d2a501102a88f202a7b6061  circuit-1912-32-256-64_hez3_0006.zkey
112bf86cbd8c538574d26fb2a3e22abbcf0c17f1e6c1f03283573f64ee337a170c71bee457367240310fb6d45206233e3cfe1e30b15eb82809e61fcd14962369  circuit-344-32-256-64_hez3_0006.zkey
9785c512aa512549981d083724f962c9b799a9a23e182909917e6ac2509a4f31910aa418ce47c9cbd3cbdb89f7c3fe058cbb4483cba9e0f90f77535466b64502  withdraw_hez3_0006.zkey
```

The circuit and contribution hashes from `snarkjs` are:

```
snarkjs zkey contribute circuit-344-32-256-64_hez3_0005.zkey circuit-344-32-256-64_hez3_0006.zkey -v -n=weijie
[INFO]  snarkJS: Circuit Hash: 
                b6b78d08 04636911 0d12afad 8c49a0e9
                5c0b03ed 99f2ff8e dedf2d51 dd427750
                2a9ca1b7 5417069e 174ce637 da105132
                ea8b5448 21ca6ade 4df911cd 52d34550
[INFO]  snarkJS: Contribution Hash: 
                e7613130 c3d333d9 e577151a aea73d38
                8fafb500 4334252d fb3fd21b f548e5c0
                fb2f91e6 b1b40d75 f1943b5c 378b669c
                9091719c cf8f1376 4fad50b1 d83d2916
```

```
snarkjs zkey contribute withdraw_hez3_0005.zkey withdraw_hez3_0006.zkey -v -n=weijie
[INFO]  snarkJS: Circuit Hash:
                26f8883b 44e999e7 dc749bac d7a914e3
                4fe4602e bb18d681 39a70cd9 16c22722
                2ec186f5 1dd876d1 04a403df 13433b27
                7c0c69a3 3a2aca64 dc3365c0 ce74a0ec
[INFO]  snarkJS: Contribution Hash:
                b36d1e18 5ddc8167 759e93f6 e08e4b72
                4ef21af4 e03054c4 a6950937 cf9c44bc
                f56faf7d 89e46f9b de77ab70 1d88facb
                b3f0dd0d 6c612345 6d32a872 df91ae8a
```

```
snarkjs zkey contribute circuit-1912-32-256-64_hez3_0005.zkey circuit-1912-32-256-64_hez3_0006.zkey -v -n=weijie
[INFO]  snarkJS: Circuit Hash: 
                07b5cfaa d2d4674e 095f20dd 11e516bc
                e8aa1d3e 59174e10 e538504d 208bc959
                5c05e470 3db00d49 212258a3 12da9230
                83a819ea 56af7132 e12996f3 13882859
[INFO]  snarkJS: Contribution Hash: 
                92723678 68e91c11 cc524870 e08587c5
                22b97748 6d8cb1c1 a219a3b4 7a8ba57b
                95f72fec f760dbd5 67d2e2ed 0896e7bd
                e210d67d 08fcd551 3f3f0b83 f5317864
```
