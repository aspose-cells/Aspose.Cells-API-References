##Enum LoadFormat
Aspose.Cells.LoadFormat enum. Represents the load file format
## LoadFormat enumeration
Represents the load file format.
```csharp
public enum LoadFormat
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Auto | `0` | Represents recognizing the format automatically. |
| Csv | `1` | Comma-Separated Values(CSV) text file. |
| CSV | `1` | Comma-Separated Values(CSV) text file. NOTE: This member is now obsolete. Instead, please use Csv property. This property will be removed 6 months later since April 2021. Aspose apologizes for any inconvenience you may have experienced. |
| Xlsx | `6` | Represents Office Open XML spreadsheetML workbook or template, with or without macros. |
| Tsv | `11` | Tab-Separated Values(TSV) text file. |
| TSV | `11` | Tab-Separated Values(TSV) text file. NOTE: This member is now obsolete. Instead, please use Tsv property. This property will be removed 6 months later since April 2021. Aspose apologizes for any inconvenience you may have experienced. |
| TabDelimited | `11` | Represents a tab delimited text file, same with Tsv. |
| Html | `12` | Represents a html file. |
| MHtml | `13` | Represents a mhtml file. |
| Ods | `14` | Open Document Sheet(ODS) file. |
| ODS | `14` | Open Document Sheet(ODS) file. NOTE: This member is now obsolete. Instead, please use Ods property. This property will be removed 6 months later since April 2021. Aspose apologizes for any inconvenience you may have experienced. |
| Excel97To2003 | `5` | Represents an Excel97-2003 xls file. |
| SpreadsheetML | `15` | Represents an Excel 2003 xml file. |
| Xlsb | `16` | Represents an xlsb file. |
| Ots | `31` | Open Document Template Sheet(OTS) file. |
| Numbers | `56` | Represents a numbers file. |
| Fods | `59` | Represents OpenDocument Flat XML Spreadsheet (.fods) file format. |
| FODS | `59` | Represents OpenDocument Flat XML Spreadsheet (.fods) file format. NOTE: This member is now obsolete. Instead, please use Fods property. This property will be removed 6 months later since April 2021. Aspose apologizes for any inconvenience you may have experienced. |
| Sxc | `60` | Represents StarOffice Calc Spreadsheet (.sxc) file format. |
| SXC | `60` | Represents StarOffice Calc Spreadsheet (.sxc) file format. NOTE: This member is now obsolete. Instead, please use Sxc property. This property will be removed 6 months later since April 2021. Aspose apologizes for any inconvenience you may have experienced. |
| Xml | `51` | Represents a simple xml file. |
| Epub | `52` | Reprents an EPUB file. |
| Azw3 | `53` | Represents an AZW3 file. |
| Chm | `54` | Represents a CHM file. |
| Markdown | `55` | Represents a Markdown file. |
| Unknown | `255` | Represents unrecognized format, cannot be loaded. |
| Image | `254` | Image |
| Json | `513` | Json |
| Dif | `30` | Data Interchange Format. |
| Dbf | `515` | Xbase Data file |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class LoadFormatDemo
{
public static void LoadFormatExample()
{
// Load an Excel file in different formats using Aspose.Cells
string[] filePaths = {
"LoadFormatDemo_original.xlsx",
"LoadFormatDemo_original.xls",
"LoadFormatDemo_original.csv",
"LoadFormatDemo_original.json"
};
foreach (var filePath in filePaths)
{
// Determine the load format based on file extension
LoadFormat loadFormat = GetLoadFormat(filePath);
// Create LoadOptions with the determined LoadFormat
LoadOptions loadOptions = new LoadOptions(loadFormat);
// Load the workbook with the specified load options
Workbook workbook = new Workbook(filePath, loadOptions);
// Perform some operations on the workbook
Console.WriteLine($"Loaded file: {filePath}");
Console.WriteLine($"Number of sheets: {workbook.Worksheets.Count}");
// Save the workbook to a new file
string outputFilePath = $"output_{System.IO.Path.GetFileName(filePath)}";
workbook.Save(outputFilePath);
Console.WriteLine($"Saved file as: {outputFilePath}");
}
}
private static LoadFormat GetLoadFormat(string filePath)
{
string extension = System.IO.Path.GetExtension(filePath).ToLower();
switch (extension)
{
case ".xlsx":
return LoadFormat.Xlsx;
case ".xls":
return LoadFormat.Excel97To2003;
case ".csv":
return LoadFormat.Csv;
case ".json":
return LoadFormat.Json;
default:
return LoadFormat.Auto;
}
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
