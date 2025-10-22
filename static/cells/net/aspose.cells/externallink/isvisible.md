##ExternalLink.IsVisible
ExternalLink property. Indicates whether this external link is visible in MS Excel
## ExternalLink.IsVisible property
Indicates whether this external link is visible in MS Excel.
```csharp
public bool IsVisible { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExternalLinkPropertyIsVisibleDemo
{
public static void Run()
{
// Create a workbook with external links
Workbook workbook = new Workbook();
// Add some data to the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("External Link Demo");
// Create a new workbook to use as external link source
Workbook externalWorkbook = new Workbook();
externalWorkbook.Worksheets[0].Cells["A1"].PutValue(100);
externalWorkbook.Save("external_data.xlsx");
// Add an external link reference
workbook.Worksheets[0].Cells["B1"].Formula = "='[external_data.xlsx]Sheet1'!A1";
// Check external links (they will be automatically created when loading formulas)
foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
{
Console.WriteLine($"External link visibility: {link.IsVisible}");
Console.WriteLine($"External link data source: {link.DataSource}");
}
// Create another workbook to demonstrate loading existing file
Workbook workbook2 = new Workbook();
workbook2.Worksheets[0].Cells["A1"].PutValue("=SUM([example.xls]Sheet1!A1:A10)");
// Save and reload to demonstrate external links
workbook2.Save("output.xlsx");
Workbook loadedWorkbook = new Workbook("output.xlsx");
// Check external links in loaded workbook
foreach (ExternalLink link in loadedWorkbook.Worksheets.ExternalLinks)
{
Console.WriteLine($"External link URL: {link.DataSource}, Visible: {link.IsVisible}");
}
}
}
}
```
### See Also
* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
