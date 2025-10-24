##LoadFormat Enum
'LoadFormat enum. Encapsulates the object that represents loadformat in Go.'
## LoadFormat Enum
Represents the load file format.
```go
type LoadFormat int32
```
## Fields
| Field | Description |
| --- | --- |
|[Auto](./auto/) | Represents recognizing the format automatically. |
|[Csv](./csv/) | Comma-Separated Values(CSV) text file. |
|[Xlsx](./xlsx/) | Represents Office Open XML spreadsheetML workbook or template, with or without macros. |
|[Tsv](./tsv/) | Tab-Separated Values(TSV) text file. |
|[Html](./html/) | Represents a html file. |
|[MHtml](./mhtml/) | Represents a mhtml file. |
|[Ods](./ods/) | Open Document Sheet(ODS) file. |
|[Excel97To2003](./excel97to2003/) | Represents an Excel97-2003 xls file. |
|[SpreadsheetML](./spreadsheetml/) | Represents an Excel 2003 xml file. |
|[Xlsb](./xlsb/) | Represents an xlsb file. |
|[Ots](./ots/) | Open Document Template Sheet(OTS) file. |
|[Numbers](./numbers/) | Represents a numbers file. |
|[Fods](./fods/) | Represents OpenDocument Flat XML Spreadsheet (.fods) file format. |
|[Sxc](./sxc/) | Represents StarOffice Calc Spreadsheet (.sxc) file format. |
|[Xml](./xml/) | Represents a simple xml file. |
|[Epub](./epub/) | Reprents an EPUB file. |
|[Azw3](./azw3/) | Represents an AZW3 file. |
|[Chm](./chm/) | Represents a CHM file. |
|[Markdown](./markdown/) | Represents a Markdown file. |
|[Unknown](./unknown/) | Represents unrecognized format, cannot be loaded. |
|[Image](./image/) | Image |
|[Json](./json/) | Json |
|[Dif](./dif/) | Data Interchange Format. |
|[Dbf](./dbf/) | Xbase Data file |
