* `await HiveDB.getdata("wif")`

* Get Clarification on all the functions of the mergeUtxos.dart

* sweepfunds.dart

* In walletinfo.dart
```
 var rootSeed = bitbox.Mnemonic.toSeed(seed);
    var masterNode = bitbox.HDNode.fromSeed(rootSeed);
    accountNode = masterNode.derivePath("m/44'/245'/0'/0");
``` 
