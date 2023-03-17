# v3-core

KODKODKOD DEX v3-core smart contract

```bash
npm install
npm run gen-binding
```

## March 17

```bash
completium-cli generate michelson ./contracts/kodexV3Pool.arl 1> ./contracts/michelson/kodexV3Pool.tz;

npm run gen-binding;
    Wrote ./tests/binding/kodexV3Factory.ts
    Wrote ./tests/binding/kodexV3Library.ts
    Wrote ./tests/binding/kodexV3MathLibrary.ts
    Wrote ./tests/binding/kodexV3Pool.ts
    Invalid file ./contracts/michelson/kodexV3Pool.tz

completium-cli deploy ./contracts/kodexV3MathLibrary.arl
    total cost    : 5.003752 ꜩ
    https://better-call.dev/ghostnet/KT1P15iyFY9d4PUqVz49Rm2TnQFqtfeGvRCe

completium-cli deploy ./contracts/kodexV3Library.arl --parameters '{"mathLib":"KT1P15iyFY9d4PUqVz49Rm2TnQFqtfeGvRCe"}'
    total cost    : 6.022538 ꜩ
    https://better-call.dev/ghostnet/KT1KSjr9YbBXzZushTS4HuJ9jjyp1j74GYCC

completium-cli deploy ./contracts/kodexV3Factory.arl --parameters '{"owner":"tz1afKmEFo11mpXr4JdodJDTXYLfw7GTFbak", "kodexV3lib":"KT1KSjr9YbBXzZushTS4HuJ9jjyp1j74GYCC"}'
    total cost    : 7.88292 ꜩ
    https://better-call.dev/ghostnet/KT1NArLsaWtJeG8Jreza1EacSaH8KAhho5Wy
```
