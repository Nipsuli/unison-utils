# Simple unison (text) utils

Install: `pull https://github.com/Nipsuli/unison-utils .utils`

Check also: [unisonlibraries](https://github.com/runarorama/unisonlibraries)


Has namespace `utils` containing following functions
``` Idris
Char.isWhiteSpace : Char -> Boolean
Text.cons : Char -> Text -> Text
Text.fromBytes : Bytes -> Text
Text.join : Text -> [Text] -> Text
Text.length : Text -> Nat
Text.snoc : Text -> Char -> Text
Text.split : Text -> Text -> [Text]
Text.splitOnce : Text -> Text -> [Text]
Text.startsWith : Text -> Text -> Boolean
Text.toBytes : Text -> Bytes
Text.trimWhiteSpace : Text -> Text
```


Following Chars are counted as whitespace:
``` Idris
whiteSpaceChars = Set.fromList (List.map Char.fromNat ([
  9, -- character tabulation U+0009
  10, -- line feed U+000A
  11, -- line tabulation U+000B
  12, -- form feed U+000C
  13, -- carriage return U+000D
  32, -- space U+0020
  133, -- next line U+0085
  160, -- no-break space U+00A0
  5760, -- ogham space mark U+1680
  8192, -- en quad U+2000
  8193, -- em quad U+2001
  8194, -- en space U+2002
  8195, -- em space U+2003
  8196, -- three-per-em space U+2004
  8197, -- four-per-em space U+2005
  8198, -- six-per-em space U+2006
  8199, -- figure space U+2007
  8200, -- punctuation space U+2008
  8201, -- thin space U+2009
  8202, -- hair space U+200A
  8232, -- line separator U+2028
  8233, -- paragraph separator U+2029
  8239, -- narrow no-break space U+202F
  8287, -- medium mathematical space U+205F
  12288, -- ideographic space U+3000
  6158, -- mongolian vowel separator U+180E
  8203, -- zero width space U+200B
  8204, -- zero width non-joiner U+200C
  8205, -- zero width joiner U+200D
  8288, -- word joiner U+2060
  65279 -- zero width non-breaking space U+FEFF
]))
```
