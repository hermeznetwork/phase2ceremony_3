# Hermez Network Second Phase2 Trusted Setup Ceremony.

NOTE: The first First Phase2 ceremony was cancelled as we added the float40
precission to the system and this implies a modification of the circuit.

This repository contains the transcript of the Phase2 Ceremony.

This ceremony runs the trusted setup for 3 circuits:

* **circuit-1912-32-256-64**
* **circuit-344-32-256-64**
* **withdraw**

The first two circuits are the validation circuits for 1912Tx and 344 Txs.  The third circuit is the one used in the rollup exits.

See [Hermez Documentation](https://docs.hermez.io/#/) for fore information of how the rollup works.

The Circom circuits can be found in [circuits](https://github.com/hermeznetwork/circuits).

For this ceremony we used the tag `phase2ceremony_3` [circuits](https://github.com/hermeznetwork/circuits) with repo commit value  `45a486464334e08bd5da948ffb2099fcf1dc7c2f`

For contributing to the ceremony see: [CONTRIBUTE.md](CONTRIBUTE.md)

For verifying the ceremony see: [VERIFY.md](VERIFY.md)

## Contributions

### 1912 Tx Circuit

| Atestation<br>&nbsp; | Contribution File<br>&nbsp; | Contributor<br>&nbsp; | Contribution Hash &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; |
|:-----|:------------ |:-----|:--------------------------------------|
| 0000_initial | [circuit-1912-32-256-64_hez3_0000.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-1912-32-256-64_hez3_0000.zkey)     | |
| [0001_jordi](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0001_jordi) | [circuit-1912-32-256-64_hez3_0001.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-1912-32-256-64_hez3_0001.zkey)     | [jordi](https://keybase.io/jbaylina)  | `8a3f5f8d 42d72ad3`<br>`1a03f99e 2f1e96a7`<br>`74320e40 a1402133`<br>`e462e7eb d245b208`<br>`5972bf46 a6631a59`<br>`b0ed85e3 efa143ad`<br>`dd8b023f 8af318ba`<br>`3f43a426 796fce83` |
| [0002_kobigurk](https://github.com/hermeznetwork/phase2ceremony_2/tree/main/0002_kobigurk) | [circuit-1912-32-256-64_hez3_0002.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-1912-32-256-64_hez3_0002.zkey)     | [kobigurk](https://keybase.io/kobigurk)  | `76f93c82 9a303b63`<br>`5486ba1e de76ce0a`<br>`050321f8 d4fe794f`<br>`d6108057 0d499a3d`<br>`02e4ae89 2429056f`<br>`83b85f57 672d74f4`<br>`a352fea0 4fa4599b`<br>`5f467b67 df6c2395` |



### 344 Tx Circuit

| Atestation<br>&nbsp; | Contribution File<br>&nbsp; | Contributor<br>&nbsp; | Contribution Hash &nbsp; &nbsp; &nbsp; &nbsp; |
|:-----|:------------ |:-----|:--------------------------------------|
| 0000_initial | [circuit-344-32-256-64_hez3_0000.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-344-32-256-64_hez3_0000.zkey)     | |
| [0001_jordi](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0001_jordi) | [circuit-344-32-256-64_hez3_0001.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-344-32-256-64_hez3_0001.zkey)     | [jordi](https://keybase.io/jbaylina)  | `e7fbbdef 2fa4da4f`<br>`2a5c62b9 726de9b8`<br>`2c2d6235 e0e5dc96`<br>`ba729970 26c4b621`<br>`90e2e19f 0c9d754a`<br>`501f4c66 b67c247c`<br>`6b33b358 6a14a801`<br>`2b858529 79c699c7` |
| [0002_kobigurk](https://github.com/hermeznetwork/phase2ceremony_2/tree/main/0002_kobigurk) | [circuit-344-32-256-64_hez3_0002.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-344-32-256-64_hez3_0002.zkey)     | [kobigurk](https://keybase.io/kobigurk)  | `4e76df2b c54af529`<br>`7f54ed51 8087676b`<br>`ba16d6e7 c843f884`<br>`9ab4472d 0881da6b`<br>`c4caa9b6 2331a497`<br>`6983ec17 4dee57ff`<br>`83059d08 90a797e5`<br>`bee57c7c 46c1acf1` |


### WithdrawCircuit

| Atestation<br>&nbsp; | Contribution File<br>&nbsp; | Contributor<br>&nbsp; | Contribution Hash &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; <br> &nbsp; |
|:-----|:------------ |:-----|:--------------------------------------|
| 0000_initial | [withdraw_hez3_0000.zkey](https://hermez.s3-eu-west-1.amazonaws.com/withdraw_hez3_0000.zkey)     | |
| [0001_jordi](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0001_jordi) | [withdraw_hez3_0001.zkey](https://hermez.s3-eu-west-1.amazonaws.com/withdraw_hez3_0001.zkey)     | [Jordi](https://keybase.io/jbaylina)  |     `810b8892 5e3fffdc`<br>`c3c589bf a9601160`<br>`53903f8e d3bb3104`<br>`db49f51b 65cee32f`<br>`2117420d 32b58ca5`<br>`85212ae8 e53d9649`<br>`d37d9b7d c4af2628`<br>`0a2f6929 7ef9cea4`|
| [0002_kobigurk](https://github.com/hermeznetwork/phase2ceremony_2/tree/main/0002_kobigurk) | [withdraw_hez3_0002.zkey](https://hermez.s3-eu-west-1.amazonaws.com/withdraw_hez3_0002.zkey)     | [kobigurk](https://keybase.io/kobigurk)  | `c4fd77a7 45ebb208`<br>`5c72db47 657ac337`<br>`8907b8cb 303c2e2e`<br>`5ad860d9 0a88190a`<br>`d1a26862 309bff02`<br>`3f3e6c2e ec64eac0`<br>`879e8752 e40d0734`<br>`d877cb6b 0f6a96e7` |


