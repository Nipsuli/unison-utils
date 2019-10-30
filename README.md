# Simple unison utils

Install: `pull https://github.com/Nipsuli/unison-utils .utils`

Has namespace `utils` containing following functions
``` Idris
Text.split : Text -> Text -> List Text
Text.join : Text -> List Text -> Text
Text.toBytes : Text -> Bytes
Text.fromBytes : Bytes -> Text
Text.length : Text -> Nat
Text.startsWith : Text -> Text -> Boolean
List.first : List t -> List t
List.head : List t -> Optional t
List.tail : List t -> List t
```
