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
Text.trim : Text -> Text
```


Following Chars are counted as whitespace:
```
character tabulation U+0009
line feed U+000A
line tabulation U+000B
form feed U+000C
carriage return U+000D
space U+0020
next line U+0085
no-break space U+00A0
ogham space mark U+1680
en quad U+2000
em quad U+2001
en space U+2002
em space U+2003
three-per-em space U+2004
four-per-em space U+2005
six-per-em space U+2006
figure space U+2007
punctuation space U+2008
thin space U+2009
hair space U+200A
line separator U+2028
paragraph separator U+2029
narrow no-break space U+202F
medium mathematical space U+205F
ideographic space U+3000
mongolian vowel separator U+180E
zero width space U+200B
zero width non-joiner U+200C
zero width joiner U+200D
word joiner U+2060
zero width non-breaking space U+FEFF
```
