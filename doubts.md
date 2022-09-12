```
    for (var i = 0; i < slpTokens.length; i++) {
      num utxos = 0;
      for (var txo in slpUtxos) {
        if (slpTokens[i]['tokenID'] == txo['tokenId']) {
          utxos = utxos + 1;
        }
        slpTokens[i]['utxos'] = utxos;
      }
    }
```
in mergeutxos.dart

* Get Clarification on all the functions of the mergeUtxos.dart
