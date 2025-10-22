##WorksheetCollection.ExternalLinks
WorksheetCollection property. Represents external links in a workbook
## WorksheetCollection.ExternalLinks property
Represents external links in a workbook.
```csharp
public ExternalLinkCollection ExternalLinks { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionPropertyExternalLinksDemo
{
public static void Run()
{
// Create a source workbook with external link
var sourceWorkbook = new Workbook();
sourceWorkbook.Worksheets.Add("Sheet1");
sourceWorkbook.Worksheets.ExternalLinks.Add("external.xlsx", new string[] { "Sheet1!A1" });
// Create a destination workbook
var destWorkbook = new Workbook();
destWorkbook.Worksheets.Add("Sheet1");
// Set external link data source
Console.WriteLine("Original external link: {0}", sourceWorkbook.Worksheets.ExternalLinks[0].DataSource);
sourceWorkbook.Worksheets.ExternalLinks[0].DataSource = "updated_external.xlsx";
Console.WriteLine("Updated external link: {0}", sourceWorkbook.Worksheets.ExternalLinks[0].DataSource);
// Save the workbook
sourceWorkbook.Save("output.xlsx");
Console.WriteLine("Workbook saved with updated external link.");
// Clean up
sourceWorkbook.Dispose();
destWorkbook.Dispose();
}
}
}
```
### See Also
* class [ExternalLinkCollection](../../externallinkcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
