##ExternalLink.DataSource
ExternalLink property. Represents data source of the external link
## ExternalLink.DataSource property
Represents data source of the external link.
```csharp
public string DataSource { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExternalLinkPropertyDataSourceDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create an external link to another workbook
worksheet.Cells["A1"].Formula = "='[external.xlsx]Sheet1'!A1";
// Save the workbook
workbook.Save("output.xlsx");
// Load the saved workbook to check external links
Workbook loadedWorkbook = new Workbook("output.xlsx");
// Access the external link's DataSource property
if (loadedWorkbook.Worksheets.ExternalLinks.Count > 0)
{
string dataSource = loadedWorkbook.Worksheets.ExternalLinks[0].DataSource;
Console.WriteLine("External link data source: " + dataSource);
}
}
}
}
```
### See Also
* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
