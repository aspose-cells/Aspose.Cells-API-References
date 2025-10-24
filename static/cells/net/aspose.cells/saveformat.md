##Enum SaveFormat
Aspose.Cells.SaveFormat enum. Represents the format in which the workbook is saved
## SaveFormat enumeration
Represents the format in which the workbook is saved.
```csharp
public enum SaveFormat
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Csv | `1` | Comma-Separated Values(CSV) text file. |
| CSV | `1` | Comma-Separated Values(CSV) text file. NOTE: This member is now obsolete. Instead, please use Csv property. This property will be removed 6 months later since April 2021. Aspose apologizes for any inconvenience you may have experienced. |
| Xlsx | `6` | Represents an xlsx file. |
| Xlsm | `7` | Represents an xlsm file which enable macros. |
| Xltx | `8` | Represents an xltx file. |
| Xltm | `9` | Represents an xltm file which enable macros. |
| Xlam | `10` | Represents an xltm file which enable addin macros. |
| Tsv | `11` | Tab-Separated Values(TSV) text file. |
| TSV | `11` | Tab-Separated Values(TSV) text file. NOTE: This member is now obsolete. Instead, please use Tsv property. This property will be removed 6 months later since April 2021. Aspose apologizes for any inconvenience you may have experienced. |
| TabDelimited | `11` | Represents a tab delimited text file, same with Tsv. |
| Html | `12` | Represents a html file. |
| MHtml | `17` | Represents a mhtml file. |
| Ods | `14` | Open Document Sheet(ODS) file. |
| ODS | `14` | Open Document Sheet(ODS) file. NOTE: This member is now obsolete. Instead, please use Ods property. This property will be removed 6 months later since April 2021. Aspose apologizes for any inconvenience you may have experienced. |
| Excel97To2003 | `5` | Represents an Excel97-2003 xls file. |
| SpreadsheetML | `15` | Represents an Excel 2003 xml file. |
| Xlsb | `16` | Represents an xlsb file. |
| Auto | `0` | If saving the file to the disk,the file format accords to the extension of the file name. If saving the file to the stream, the file format is xlsx. |
| Unknown | `255` | Represents unrecognized format, cannot be saved. |
| Pdf | `13` | Represents a Pdf file. |
| Xps | `20` | XPS (XML Paper Specification) format. |
| XPS | `20` | XPS (XML Paper Specification) format. NOTE: This member is now obsolete. Instead, please use Xps property. This property will be removed 6 months later since April 2021. Aspose apologizes for any inconvenience you may have experienced. |
| Tiff | `21` | Represents a TIFF file. |
| TIFF | `21` | Represents a TIFF file. NOTE: This member is now obsolete. Instead, please use Tiff property. This property will be removed 6 months later since April 2021. Aspose apologizes for any inconvenience you may have experienced. |
| Svg | `28` | SVG file. |
| SVG | `28` | SVG file. NOTE: This member is now obsolete. Instead, please use Svg property. This property will be removed 6 months later since April 2021. Aspose apologizes for any inconvenience you may have experienced. |
| Dif | `30` | Data Interchange Format. |
| Ots | `31` | Open Document Template Sheet(OTS) file. |
| Xlt | `32` | Excel 97-2003 template file. |
| Xml | `51` | Represents a simple xml file. |
| Numbers | `56` | Represents a numbers file. |
| Markdown | `57` | Represents markdown document. |
| Fods | `59` | Represents OpenDocument Flat XML Spreadsheet (.fods) file format. |
| FODS | `59` | Represents OpenDocument Flat XML Spreadsheet (.fods) file format. NOTE: This member is now obsolete. Instead, please use Fods property. This property will be removed 6 months later since April 2021. Aspose apologizes for any inconvenience you may have experienced. |
| Sxc | `60` | Represents StarOffice Calc Spreadsheet (.sxc) file format. |
| SXC | `60` | Represents StarOffice Calc Spreadsheet (.sxc) file format. NOTE: This member is now obsolete. Instead, please use Sxc property. This property will be removed 6 months later since April 2021. Aspose apologizes for any inconvenience you may have experienced. |
| Pptx | `61` | Represents .pptx file. |
| Docx | `62` | Represents .docx file. |
| Emf | `258` | Windows Enhanced Metafile. |
| Jpg | `261` | JPEG JFIF. |
| Png | `262` | Portable Network Graphics. |
| Bmp | `263` | Windows Bitmap |
| Gif | `322` | Gif |
| Json | `513` | Json |
| SqlScript | `514` | Sql |
| XHtml | `771` | Rrepesents XHtml file. please use [`HtmlVersion`](../htmlsaveoptions/htmlversion/) property. This property will be removed 6 months later since March 2025. Aspose apologizes for any inconvenience you may have experienced. |
| Epub | `772` | Represents Epub file. |
| Azw3 | `773` | Represents Azw3 file. |
| Pcl | `1025` | PCL (Printer Command Language) |
| Dbf | `515` | Xbase Data file |
### Examples
```csharp
using Aspose.Cells;
using System;
namespace AsposeCellsExamples
{
public class SaveFormatDemo
{
public static void SaveFormatExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["A3"].PutValue("Jane");
worksheet.Cells["A4"].PutValue("Doe");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["B3"].PutValue(25);
worksheet.Cells["B4"].PutValue(35);
// Save the workbook in different formats
workbook.Save("SaveFormatExample.xlsx", SaveFormat.Xlsx);
workbook.Save("SaveFormatExample.xls", SaveFormat.Excel97To2003);
workbook.Save("SaveFormatExample.csv", SaveFormat.Csv);
workbook.Save("SaveFormatExample.pdf", SaveFormat.Pdf);
workbook.Save("SaveFormatExample.html", SaveFormat.Html);
// Output the results
Console.WriteLine("Workbook saved in multiple formats.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
