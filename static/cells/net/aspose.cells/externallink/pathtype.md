##ExternalLink.PathType
ExternalLink property. Get the path type of this external link
## ExternalLink.PathType property
Get the path type of this external link
```csharp
public string PathType { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExternalLinkPropertyPathTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet
Worksheet sheet = workbook.Worksheets[0];
// Create an external link to another workbook
sheet.Cells["A1"].Formula = "='C:\\Temp\\ExternalWorkbook.xlsx'!Sheet1!A1";
// Get the external link
ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
// Display the path type of the external link
Console.WriteLine("Path Type: " + externalLink.PathType);
// Save the workbook
workbook.Save("ExternalLinkDemo.xlsx");
}
}
}
```
### See Also
* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
