##Enum DirectoryType
Aspose.Cells.DirectoryType enum. Represents the directory type of the file name
## DirectoryType enumeration
Represents the directory type of the file name.
```csharp
public enum DirectoryType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Volume | `0` | Represents an MS-DOS drive letter. It is followed by the drive letter. Or UNC file names, such as \\server\share\myfile.xls |
| SameVolume | `1` | Indicates that the source workbook is on the same drive as the dependent workbook (the drive letter is omitted) |
| DownDirectory | `2` | Indicates that the source workbook is in a subdirectory of the current directory. |
| UpDirectory | `3` | Indicates that the source workbook is in the parent directory of the current directory. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class DirectoryTypeDemo
{
public static void DirectoryTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Data");
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(200);
worksheet.Cells["A4"].PutValue(300);
// Add an external link to the workbook
string externalFileName = "externalWorkbook.xlsx";
string[] sheetNames = { "Sheet1" };
// Add external link with DirectoryType.Volume
int linkIndex = workbook.Worksheets.ExternalLinks.Add(DirectoryType.Volume, externalFileName, sheetNames);
// Retrieve the added external link
ExternalLink externalLink = workbook.Worksheets.ExternalLinks[linkIndex];
// Output the details of the external link
Console.WriteLine("External Link Details:");
Console.WriteLine("File Name: " + externalLink.DataSource);
// Save the workbook
workbook.Save("DirectoryTypeExample.xlsx");
workbook.Save("DirectoryTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
