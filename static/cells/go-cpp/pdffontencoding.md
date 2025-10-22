##PdfFontEncoding Enum
'PdfFontEncoding enum. Encapsulates the object that represents pdffontencoding in Go.'
## PdfFontEncoding Enum
Represents pdf embedded font encoding.
```go
type PdfFontEncoding int32
```
## Fields
| Field | Description |
| --- | --- |
|[Identity](./identity/) | Represents use Identity-H encoding for all embedded fonts in pdf. |
|[AnsiPrefer](./ansiprefer/) | Represents prefer to use WinAnsiEncoding for TrueType fonts with characters 32-127,otherwise, Identity-H encoding will be used for embedded fonts in pdf. |
