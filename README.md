# initial-ae-balances-generator-etherscan
Generate an `accounts.json` for the æeternity Mainnet genesis block.

```
$ head accounts.json
{
  "ak_2CC81QrxVxYD5T8eJcAUwJsfSRBS2fA1MpsccLRjJumZdFuD8g": 1162000000000000000,
    "ak_2ruXgsLy9jMwEqsgyQgEsxw8chYDfv2QyBfCsR6qtpQYkektWB": 5307138661548760000000,
    "ak_2r6Mmd53BTd2rRuYnV2KfLeGMmxAZJo8g79bfDMW2uBdWe4ax": 1444554454444446550,
    "ak_CGBUVnsR9EyAGz8iwdBgy6gNpKnCsZatDkmSnFogR1LTJSnMr": 3000000000000000000,
    "ak_2Zp5KWiMLT63G3kXM9jXw3yzfLqTeL9m8TyqqY2aQmKD7o3ap6": 204000000000000000000,
    "ak_2WXFcbPPFCgxgXmduQGDywfhGFRfe2GkkTjWKEEbf8jQQ44ZaC": 100000000000000000,
    "ak_f37nhJ2NyLR2LGb5PG9mGnYfLYLC2z2eFDkZFDrERYSo6zoLR": 123556789000000000,
    "ak_DJim8QGrk72aG7bDMkszdLPYfDL3AVhjvHcjPbrriDFWSTSgV": 500000000000000000,
    "ak_REvrRjqYYJWTGr2JikZiem2g1qfqBdb2fQ8pwmKVWHM2uLaV5": 500000000000000000000,
$
```

# Usage

`node initial-balances-generator-etherscan.js -k XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX`

where: `-k [Etherscan.io api key]`

# Verify

Verify sha256 of `accounts.json`

```
$ shasum -a 256 accounts.json

6b5895bc9fcad63880f465ce841edb5cd4ae313c53bd39289da9ce64f263fd74  accounts.json
```
