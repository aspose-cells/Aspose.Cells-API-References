##Enum FileFormatType
Aspose.Cells.FileFormatType enum. Represents the file format types
## FileFormatType enumeration
Represents the file format types.
```csharp
public enum FileFormatType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Csv | `1` | Comma-Separated Values(CSV) text file. |
| Xlsx | `6` | Office Open XML SpreadsheetML file (macro-free). |
| Xlsm | `7` | Office Open XML SpreadsheetML Macro-Enabled file. |
| Xltx | `8` | Office Open XML SpreadsheetML Template (macro-free). |
| Xltm | `9` | Office Open XML SpreadsheetML Macro-Enabled Template. |
| Xlam | `10` | Office Open XML SpreadsheetML addinMacro-Enabled file. |
| Tsv | `11` | Tab-Separated Values(TSV) text file. |
| TabDelimited | `11` | Tab-Separated Values(TSV) text file, same with Tsv. |
| Html | `12` | HTML format. |
| MHtml | `17` | MHTML (Web archive) format. |
| Ods | `14` | Open Document Sheet(ODS) file. |
| Excel97To2003 | `5` | Excel97-2003 spreadsheet file. |
| SpreadsheetML | `15` | Excel 2003 XML Data file. |
| Xlsb | `16` | The Excel Binary File Format (.xlsb) |
| Unknown | `255` | Represents unrecognized format, cannot be loaded. |
| Pdf | `13` | PDF (Adobe Portable Document) format. |
| Xps | `20` | XPS (XML Paper Specification) format. |
| Tiff | `21` | Represents a TIFF file. |
| Svg | `28` | SVG file. |
| Excel95 | `22` | Represents an Excel95 xls file. |
| Excel4 | `23` | Represents an Excel4.0 xls file. |
| Excel3 | `24` | Represents an Excel3.0 xls file. |
| Excel2 | `25` | Represents an Excel2.1 xls file. |
| Pptx | `26` | Represents a pptx file. |
| Docx | `27` | Represents a docx file. |
| Dif | `30` | Data Interchange Format. |
| Doc | `31` | Represents a doc file. |
| Ppt | `32` | Represents a ppt file. |
| MapiMessage | `33` | Represents a email file. |
| MsEquation | `34` | Represents the MS Equation 3.0 object. |
| Ole10Native | `35` | Represents the embedded native object. |
| Vsd | `36` | Represents MS Visio VSD binary format. |
| Vsdx | `37` | Represents MS Visio 2013 VSDX file format. |
| Docm | `38` | Represents a docm file. |
| Dotx | `39` | Represents a dotx file. |
| Dotm | `40` | Represents a dotm file. |
| Pptm | `41` | Represents a pptm file. |
| Potx | `42` | Represents a Potx file. |
| Potm | `43` | Represents a Potm file. |
| Ppsx | `44` | Represents a ppsx file. |
| Ppsm | `45` | Represents a ppsm file. |
| Ooxml | `46` | Represents office open xml file(such as xlsx, docx,pptx, etc). |
| Odt | `47` | Represents an ODT file. |
| Odp | `48` | Represents a ODP file. |
| Odf | `49` | Represents an ODF file. |
| Odg | `50` | Represents an ODG file. |
| Xml | `51` | Represents a simple xml file. |
| Xlt | `52` | Excel97-2003 spreadsheet template. |
| Ott | `53` | Represents an OTT file. |
| Bmp | `54` | Represents a BMP file. |
| Ots | `55` | Represents an ots file. |
| Numbers | `56` | Represents Numbers 9.0 file format by Apple Inc. |
| Numbers09 | `56` | Represents Numbers 9.0 file format by Apple Inc. |
| Markdown | `57` | Represents markdown document. |
| GraphChart | `58` | Represents embedded graph chart. |
| Fods | `59` | Represents OpenDocument Flat XML Spreadsheet (.fods) file format. |
| Sxc | `60` | Represents StarOffice Calc Spreadsheet (.sxc) file format. |
| Otp | `61` | Represents a OTP file. |
| Numbers35 | `62` | Represents Numbers 3.5 file format since 2014 by Apple Inc |
| Ole | `64` | Represents the embedded ole object. |
| Emf | `258` | Windows Enhanced Metafile. |
| Wmf | `259` | Windows Metafile. |
| Jpg | `261` | JPEG JFIF. |
| Png | `262` | Portable Network Graphics. |
| Gif | `322` | Gif |
| WebP | `323` | Webp |
| Json | `513` | Json |
| SqlScript | `514` | Sql |
| Dbf | `515` | Xbase Data file |
| FlatOpc | `516` | Flat opc file |
| XHtml | `771` | Rrepesents XHtml file. |
| OneNote | `772` | Rrepesents One Note file. |
| MicrosoftCabinet | `773` | Rrepesents Microsoft Cabinet file. |
| Rtf | `774` | Rtf |
| Epub | `775` | EPUB |
| Azw3 | `777` | AZW3 |
| Chm | `784` | CHM |
| Oxps | `776` | OXPS (Open XML Paper Specification) format. |
| GZip | `35615` | Rrepesents GZip file. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FileFormatTypeDemo
{
public static void FileFormatTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Set the name of the worksheet
worksheet.Name = "File Format Example";
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("File Format Type");
worksheet.Cells["A2"].PutValue(FileFormatType.Csv);
worksheet.Cells["A3"].PutValue(FileFormatType.Xlsx);
worksheet.Cells["A4"].PutValue(FileFormatType.Pdf);
worksheet.Cells["A5"].PutValue(FileFormatType.Xlsm);
// Output the file format types
for (int i = 2; i <= 5; i++)
{
var fileFormat = worksheet.Cells[$"A{i}"].StringValue;
Console.WriteLine($"Row {i}: {fileFormat}");
}
// Save the workbook
workbook.Save("FileFormatTypeExample.xlsx");
workbook.Save("FileFormatTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
