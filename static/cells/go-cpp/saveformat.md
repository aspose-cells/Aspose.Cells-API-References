##SaveFormat Enum
'SaveFormat enum. Encapsulates the object that represents saveformat in Go.'
## SaveFormat Enum
Represents the format in which the workbook is saved.
```go
type SaveFormat int32
```
## Fields
| Field | Description |
| --- | --- |
|[Csv](./csv/) | Comma-Separated Values(CSV) text file. |
|[Xlsx](./xlsx/) | Represents an xlsx file. |
|[Xlsm](./xlsm/) | Represents an xlsm file which enable macros. |
|[Xltx](./xltx/) | Represents an xltx file. |
|[Xltm](./xltm/) | Represents an xltm file which enable macros. |
|[Xlam](./xlam/) | Represents an xltm file which enable addin macros. |
|[Tsv](./tsv/) | Tab-Separated Values(TSV) text file. |
|[Html](./html/) | Represents a html file. |
|[MHtml](./mhtml/) | Represents a mhtml file. |
|[Ods](./ods/) | Open Document Sheet(ODS) file. |
|[Excel97To2003](./excel97to2003/) | Represents an Excel97-2003 xls file. |
|[SpreadsheetML](./spreadsheetml/) | Represents an Excel 2003 xml file. |
|[Xlsb](./xlsb/) | Represents an xlsb file. |
|[Auto](./auto/) | If saving the file to the disk,the file format accords to the extension of the file name.If saving the file to the stream, the file format is xlsx. |
|[Unknown](./unknown/) | Represents unrecognized format, cannot be saved. |
|[Pdf](./pdf/) | Represents a Pdf file. |
|[Xps](./xps/) | XPS (XML Paper Specification) format. |
|[Tiff](./tiff/) | Represents a TIFF file. |
|[Svg](./svg/) | SVG file. |
|[Dif](./dif/) | Data Interchange Format. |
|[Ots](./ots/) | Open Document Template Sheet(OTS) file. |
|[Xlt](./xlt/) | Excel 97-2003 template file. |
|[Xml](./xml/) | Represents a simple xml file. |
|[Numbers](./numbers/) | Represents a numbers file. |
|[Markdown](./markdown/) | Represents markdown document. |
|[Fods](./fods/) | Represents OpenDocument Flat XML Spreadsheet (.fods) file format. |
|[Sxc](./sxc/) | Represents StarOffice Calc Spreadsheet (.sxc) file format. |
|[Pptx](./pptx/) | Represents .pptx file. |
|[Docx](./docx/) | Represents .docx file. |
|[Emf](./emf/) | Windows Enhanced Metafile. |
|[Jpg](./jpg/) | JPEG JFIF. |
|[Png](./png/) | Portable Network Graphics. |
|[Bmp](./bmp/) | Windows Bitmap |
|[Gif](./gif/) | Gif |
|[Json](./json/) | Json |
|[SqlScript](./sqlscript/) | Sql |
|[Epub](./epub/) | Represents Epub file. |
|[Azw3](./azw3/) | Represents Azw3 file. |
|[Pcl](./pcl/) | PCL (Printer Command Language) |
|[Dbf](./dbf/) | Xbase Data file |
