# Simple unison utils

Install: `pull https://github.com/Nipsuli/unison-utils .utils`

Check: [unisonlibraries](https://github.com/runarorama/unisonlibraries)


Has namespace `utils` containing following functions
``` Idris
Text.cons : Char -> Text -> Text
Text.fromBytes : Bytes -> Text
Text.join : Text -> [Text] -> Text
Text.length : Text -> Nat
Text.snoc : Text -> Char -> Text
Text.split : Text -> Text -> [Text]
Text.split1 : Text -> Text -> [Text]
Text.startsWith : Text -> Text -> Boolean
Text.toBytes : Text -> Bytes
```
