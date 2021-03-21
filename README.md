# Hermez Network Third Phase2 Trusted Setup Ceremony.

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
| [0003_eduadiez](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0003_eduadiez) | [circuit-1912-32-256-64_hez3_0003.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-1912-32-256-64_hez3_0003.zkey)     | [eduadiez](https://keybase.io/eduadiez)  | `9c27638e 3a3a2cd2`<br>`16cadf13 c9407b09`<br>`24248cd8 c4cfd64e`<br>`9b927bed 84164044`<br>`cb9cdf1f 6b2b9caf`<br>`e8e4969a 2e90b6bb`<br>`7aa76e3f 7f8c82d4`<br>`ea6efecc 825fcfa5` |
| [0004_hildebrandtthore](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0004_hildebrandtthore) | [circuit-1912-32-256-64_hez3_0004.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-1912-32-256-64_hez3_0004.zkey)     | [thore1234](https://keybase.io/thore1234)  | `84a1a210 4ea0eb21`<br>`22116144 e298a998`<br>`3f4f1951 ba0e48ee`<br>`9920ee37 c714e632`<br>`a511565f d6deaa73`<br>`e3016fcd 3437bf79`<br>`4f78418d 78565666`<br>`c92989bc 52b59651` |
| [0005_josephc](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0005_josephc) | [circuit-1912-32-256-64_hez3_0005.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-1912-32-256-64_hez3_0005.zkey)     | [josephc](https://keybase.io/cdili)  | `44c9badc be70b3d5`<br>`4870bff2 46431b99`<br>`91f66552 8a6ead32`<br>`baaa2ff8 93100abb`<br>`57726aac e59977ce`<br>`86560adb 3cac5d2e`<br>`cd1f8ca0 b6431d04`<br>`726d80a1 c96f4b9a` |
| [0006_weijie](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0006_weijie) | [circuit-1912-32-256-64_hez3_0006.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-1912-32-256-64_hez3_0006.zkey)     | [contactkohweijie](https://keybase.io/contactkohweijie)  | `92723678 68e91c11`<br>`cc524870 e08587c5`<br>`22b97748 6d8cb1c1`<br>`a219a3b4 7a8ba57b`<br>`95f72fec f760dbd5`<br>`67d2e2ed 0896e7bd`<br>`e210d67d 08fcd551`<br>`3f3f0b83 f5317864` |
| [0007_jarrad](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0007_jarrad) | [circuit-1912-32-256-64_hez3_0007.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-1912-32-256-64_hez3_0007.zkey)     | [jarradhope](https://keybase.io/jarradhope)  | `19a14cdb f1ec8e99`<br>`3114c055 27ff10a9`<br>`db6f96f6 10f711b5`<br>`d6edee02 26b00c14`<br>`ad1821d8 9ec03817`<br>`b449631f 6a5481fa`<br>`2eaaadcb c48f45ea`<br>`231fca07 d1ae3a73` |


### 344 Tx Circuit

| Atestation<br>&nbsp; | Contribution File<br>&nbsp; | Contributor<br>&nbsp; | Contribution Hash &nbsp; &nbsp; &nbsp; &nbsp; |
|:-----|:------------ |:-----|:--------------------------------------|
| 0000_initial | [circuit-344-32-256-64_hez3_0000.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-344-32-256-64_hez3_0000.zkey)     | |
| [0001_jordi](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0001_jordi) | [circuit-344-32-256-64_hez3_0001.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-344-32-256-64_hez3_0001.zkey)     | [jordi](https://keybase.io/jbaylina)  | `e7fbbdef 2fa4da4f`<br>`2a5c62b9 726de9b8`<br>`2c2d6235 e0e5dc96`<br>`ba729970 26c4b621`<br>`90e2e19f 0c9d754a`<br>`501f4c66 b67c247c`<br>`6b33b358 6a14a801`<br>`2b858529 79c699c7` |
| [0002_kobigurk](https://github.com/hermeznetwork/phase2ceremony_2/tree/main/0002_kobigurk) | [circuit-344-32-256-64_hez3_0002.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-344-32-256-64_hez3_0002.zkey)     | [kobigurk](https://keybase.io/kobigurk)  | `4e76df2b c54af529`<br>`7f54ed51 8087676b`<br>`ba16d6e7 c843f884`<br>`9ab4472d 0881da6b`<br>`c4caa9b6 2331a497`<br>`6983ec17 4dee57ff`<br>`83059d08 90a797e5`<br>`bee57c7c 46c1acf1` |
| [0003_eduadiez](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0003_eduadiez) | [circuit-344-32-256-64_hez3_0003.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-344-32-256-64_hez3_0003.zkey)     | [eduadiez](https://keybase.io/eduadiez)  | `0f8e70b9 a5c20ee9`<br>`860647af baa06482`<br>`13746633 8ab4b038`<br>`c9159a34 0d168292`<br>`15d37871 e599f4c7`<br>`eec53814 27408cd2`<br>`4e03075b dcef4179`<br>`cce21559 9a605150` |
| [0004_hildebrandtthore](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0004_hildebrandtthore) | [circuit-344-32-256-64_hez3_0004.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-344-32-256-64_hez3_0004.zkey)     | [thore1234](https://keybase.io/thore1234)  | `bb1bab28 a8e33f75`<br>`26bf1783 9e1eccb2`<br>`aa122bbc 80d87604`<br>`44576775 a0a639e3`<br>`c80cc251 b5261b84`<br>`be25e77e 1512872a`<br>`abfe62ac 86550fdd`<br>`e26a0164 b521626c` |
| [0005_josephc](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0005_josephc) | [circuit-344-32-256-64_hez3_0005.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-344-32-256-64_hez3_0005.zkey)     | [josephc](https://keybase.io/cdili)  | `6df0aac7 9d4521ff`<br>`ea219486 c12f6682`<br>`fae28437 27720807`<br>`e1d5d06b c88170ab`<br>`37f63888 d0e4bae0`<br>`d440f9d7 9a906c6d`<br>`77d89ba0 c427af37`<br>`5bedcb96 a54a46a7` |
| [0006_weijie](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0006_weijie) | [circuit-344-32-256-64_hez3_0006.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-344-32-256-64_hez3_0006.zkey)     | [contactkohweijie](https://keybase.io/contactkohweijie)  | `e7613130 c3d333d9`<br>`e577151a aea73d38`<br>`8fafb500 4334252d`<br>`fb3fd21b f548e5c0`<br>`fb2f91e6 b1b40d75`<br>`f1943b5c 378b669c`<br>`9091719c cf8f1376`<br>`4fad50b1 d83d2916` |
| [0007_jarrad](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0007_jarrad) | [circuit-344-32-256-64_hez3_0007.zkey](https://hermez.s3-eu-west-1.amazonaws.com/circuit-344-32-256-64_hez3_0007.zkey)     | [jarradhope](https://keybase.io/jarradhope)  | `82af1ea9 809f7022`<br>`418fe8c7 2f26d089`<br>`1a163d51 d014bfb1`<br>`b4f0c827 f6266a09`<br>`d9fd268e 263a37b8`<br>`7336018f 8bd68759`<br>`b4804915 d49d1e7a`<br>`c479f637 149fe328` |


### WithdrawCircuit

| Atestation<br>&nbsp; | Contribution File<br>&nbsp; | Contributor<br>&nbsp; | Contribution Hash &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; <br> &nbsp; |
|:-----|:------------ |:-----|:--------------------------------------|
| 0000_initial | [withdraw_hez3_0000.zkey](https://hermez.s3-eu-west-1.amazonaws.com/withdraw_hez3_0000.zkey)     | |
| [0001_jordi](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0001_jordi) | [withdraw_hez3_0001.zkey](https://hermez.s3-eu-west-1.amazonaws.com/withdraw_hez3_0001.zkey)     | [Jordi](https://keybase.io/jbaylina)  |     `810b8892 5e3fffdc`<br>`c3c589bf a9601160`<br>`53903f8e d3bb3104`<br>`db49f51b 65cee32f`<br>`2117420d 32b58ca5`<br>`85212ae8 e53d9649`<br>`d37d9b7d c4af2628`<br>`0a2f6929 7ef9cea4`|
| [0002_kobigurk](https://github.com/hermeznetwork/phase2ceremony_2/tree/main/0002_kobigurk) | [withdraw_hez3_0002.zkey](https://hermez.s3-eu-west-1.amazonaws.com/withdraw_hez3_0002.zkey)     | [kobigurk](https://keybase.io/kobigurk)  | `c4fd77a7 45ebb208`<br>`5c72db47 657ac337`<br>`8907b8cb 303c2e2e`<br>`5ad860d9 0a88190a`<br>`d1a26862 309bff02`<br>`3f3e6c2e ec64eac0`<br>`879e8752 e40d0734`<br>`d877cb6b 0f6a96e7` |
| [0003_eduadiez](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0003_eduadiez) | [withdraw_hez3_0003.zkey](https://hermez.s3-eu-west-1.amazonaws.com/withdraw_hez3_0003.zkey)     | [eduadiez](https://keybase.io/eduadiez)  | `f4e21288 c2bee0e0`<br>`ca455ab0 4e9de36b`<br>`1a7be99f 129206b2`<br>`7479d8e9 afce1567`<br>`6f14d966 e601389f`<br>`5fae3780 5c07106c`<br>`868b0b63 399e379d`<br>`3cc1af1b 7ed1ecfa` |
| [0004_hildebrandtthore](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0004_hildebrandtthore) | [withdraw_hez3_0004.zkey](https://hermez.s3-eu-west-1.amazonaws.com/withdraw_hez3_0004.zkey)     | [thore1234](https://keybase.io/thore1234)  | `923804e7 581b7401`<br>`f7a43922 cb2c7898`<br>`a827965c f6d73dcc`<br>`361c991c d7453d0b`<br>`c41c5afa 99242e7b`<br>`b9ee2dec dac189fb`<br>`8ec2e78e 732730bf`<br>`270f2ab0 adc03ccd` |
| [0005_josephc](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0005_josephc) | [withdraw_hez3_0005.zkey](https://hermez.s3-eu-west-1.amazonaws.com/withdraw_hez3_0005.zkey)     | [josephc](https://keybase.io/cdili)  | `83eda87e 74b2c4a9`<br>`187a7652 42c19ae0`<br>`3393b9b9 487afd21`<br>`5c5f88ff 6a8b6318`<br>`082e204d 50d16ed1`<br>`53b243a3 d2a4c91e`<br>`3f416d8b 807eba25`<br>`de1a8b4a eb45286a` |
| [0006_weijie](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0006_weijie) | [withdraw_hez3_0006.zkey](https://hermez.s3-eu-west-1.amazonaws.com/withdraw_hez3_0006.zkey)     | [contactkohweijie](https://keybase.io/contactkohweijie)  | `b36d1e18 5ddc8167`<br>`759e93f6 e08e4b72`<br>`4ef21af4 e03054c4`<br>`a6950937 cf9c44bc`<br>`f56faf7d 89e46f9b`<br>`de77ab70 1d88facb`<br>`b3f0dd0d 6c612345`<br>`6d32a872 df91ae8a` |
| [0007_jarrad](https://github.com/hermeznetwork/phase2ceremony_3/tree/main/0007_jarrad) | [withdraw_hez3_0007.zkey](https://hermez.s3-eu-west-1.amazonaws.com/withdraw_hez3_0007.zkey)     | [jarradhope](https://keybase.io/jarradhope)  | `28d0e8fe 1d98b3bb`<br>`9ec1c2ec d199497b`<br>`cd5657c0 f9bd1253`<br>`5b7bce4f 387c04c4`<br>`6995f2f7 1505243d`<br>`756ae9df ebd1fc47`<br>`f0f3b2c7 11cabbe1`<br>`3f610e1f 6fb658c9` |


