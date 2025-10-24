##ExternalLink.Type
ExternalLink property. Gets the type of external link
## ExternalLink.Type property
Gets the type of external link.
```csharp
public ExternalLinkType Type { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExternalLinkPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet
Worksheet sheet = workbook.Worksheets[0];
// Create an external link to another workbook
sheet.Cells["A1"].Formula = "='[link.xls]Sheet1'!A1";
// Get the external link
ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
// Display the type of external link
Console.WriteLine("External Link Type: " + externalLink.Type);
// Change the external link's data source
externalLink.DataSource = "d:\\link.xls";
// Save the workbook
workbook.Save("ExternalLinkTypeExample.xlsx");
}
}
}
```
### See Also
* enum [ExternalLinkType](../../externallinktype/)
* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
