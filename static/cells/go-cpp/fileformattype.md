##FileFormatType Enum
'FileFormatType enum. Encapsulates the object that represents fileformattype in Go.'
## FileFormatType Enum
Represents the file format types.
```go
type FileFormatType int32
```
## Fields
| Field | Description |
| --- | --- |
|[Csv](./csv/) | Comma-Separated Values(CSV) text file. |
|[Xlsx](./xlsx/) | Office Open XML SpreadsheetML file (macro-free). |
|[Xlsm](./xlsm/) | Office Open XML SpreadsheetML Macro-Enabled file. |
|[Xltx](./xltx/) | Office Open XML SpreadsheetML Template (macro-free). |
|[Xltm](./xltm/) | Office Open XML SpreadsheetML Macro-Enabled Template. |
|[Xlam](./xlam/) | Office Open XML SpreadsheetML addinMacro-Enabled file. |
|[Tsv](./tsv/) | Tab-Separated Values(TSV) text file. |
|[Html](./html/) | HTML format. |
|[MHtml](./mhtml/) | MHTML (Web archive) format. |
|[Ods](./ods/) | Open Document Sheet(ODS) file. |
|[Excel97To2003](./excel97to2003/) | Excel97-2003 spreadsheet file. |
|[SpreadsheetML](./spreadsheetml/) | Excel 2003 XML Data file. |
|[Xlsb](./xlsb/) | The Excel Binary File Format (.xlsb) |
|[Unknown](./unknown/) | Represents unrecognized format, cannot be loaded. |
|[Pdf](./pdf/) | PDF (Adobe Portable Document) format. |
|[Xps](./xps/) | XPS (XML Paper Specification) format. |
|[Tiff](./tiff/) | Represents a TIFF file. |
|[Svg](./svg/) | SVG file. |
|[Excel95](./excel95/) | Represents an Excel95 xls file. |
|[Excel4](./excel4/) | Represents an Excel4.0 xls file. |
|[Excel3](./excel3/) | Represents an Excel3.0 xls file. |
|[Excel2](./excel2/) | Represents an Excel2.1 xls file. |
|[Pptx](./pptx/) | Represents a pptx file. |
|[Docx](./docx/) | Represents a docx file. |
|[Dif](./dif/) | Data Interchange Format. |
|[Doc](./doc/) | Represents a doc file. |
|[Ppt](./ppt/) | Represents a ppt file. |
|[MapiMessage](./mapimessage/) | Represents a email file. |
|[MsEquation](./msequation/) | Represents the MS Equation 3.0 object. |
|[Ole10Native](./ole10native/) | Represents the embedded native object. |
|[Vsd](./vsd/) | Represents MS Visio VSD binary format. |
|[Vsdx](./vsdx/) | Represents MS Visio 2013 VSDX file format. |
|[Docm](./docm/) | Represents a docm file. |
|[Dotx](./dotx/) | Represents a dotx file. |
|[Dotm](./dotm/) | Represents a dotm file. |
|[Pptm](./pptm/) | Represents a pptm file. |
|[Potx](./potx/) | Represents a Potx file. |
|[Potm](./potm/) | Represents a Potm file. |
|[Ppsx](./ppsx/) | Represents a ppsx file. |
|[Ppsm](./ppsm/) | Represents a ppsm file. |
|[Ooxml](./ooxml/) | Represents office open xml file(such as xlsx, docx,pptx, etc). |
|[Odt](./odt/) | Represents an ODT file. |
|[Odp](./odp/) | Represents a ODP file. |
|[Odf](./odf/) | Represents an ODF file. |
|[Odg](./odg/) | Represents an ODG file. |
|[Xml](./xml/) | Represents a simple xml file. |
|[Xlt](./xlt/) | Excel97-2003 spreadsheet template. |
|[Ott](./ott/) | Represents an OTT file. |
|[Bmp](./bmp/) | Represents a BMP file. |
|[Ots](./ots/) | Represents an ots file. |
|[Numbers09](./numbers09/) | Represents Numbers 9.0 file format by Apple Inc. |
|[Markdown](./markdown/) | Represents markdown document. |
|[GraphChart](./graphchart/) | Represents embedded graph chart. |
|[Fods](./fods/) | Represents OpenDocument Flat XML Spreadsheet (.fods) file format. |
|[Sxc](./sxc/) | Represents StarOffice Calc Spreadsheet (.sxc) file format. |
|[Otp](./otp/) | Represents a OTP file. |
|[Numbers35](./numbers35/) | Represents Numbers 3.5 file format since 2014 by Apple Inc |
|[Ole](./ole/) | Represents the embedded ole object. |
|[Emf](./emf/) | Windows Enhanced Metafile. |
|[Wmf](./wmf/) | Windows Metafile. |
|[Jpg](./jpg/) | JPEG JFIF. |
|[Png](./png/) | Portable Network Graphics. |
|[Gif](./gif/) | Gif |
|[WebP](./webp/) | Webp |
|[Json](./json/) | Json |
|[SqlScript](./sqlscript/) | Sql |
|[Dbf](./dbf/) | Xbase Data file |
|[FlatOpc](./flatopc/) | Flat opc file |
|[XHtml](./xhtml/) | Rrepesents XHtml file. |
|[OneNote](./onenote/) | Rrepesents One Note file. |
|[MicrosoftCabinet](./microsoftcabinet/) | Rrepesents Microsoft Cabinet file. |
|[Rtf](./rtf/) | Rtf |
|[Epub](./epub/) | EPUB |
|[Azw3](./azw3/) | AZW3 |
|[Chm](./chm/) | CHM |
|[Oxps](./oxps/) | OXPS (Open XML Paper Specification) format. |
|[GZip](./gzip/) | Rrepesents GZip file. |
