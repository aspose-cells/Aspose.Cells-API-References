##Workbook.UpdateLinkedDataSource
Workbook method. If this workbook contains external links to other data source Aspose.Cells will attempt to retrieve the latest data from give sources
## Workbook.UpdateLinkedDataSource method
If this workbook contains external links to other data source, Aspose.Cells will attempt to retrieve the latest data from give sources.
```csharp
public void UpdateLinkedDataSource(Workbook[] externalWorkbooks)
```
| Parameter | Type | Description |
| --- | --- | --- |
| externalWorkbooks | Workbook[] | Workbooks that will be used to update data of external links referenced by this workbook. The match of those workbooks with external links is determined by [`FileName`](../filename/) and [`DataSource`](../../externallink/datasource/). So please make sure [`FileName`](../filename/) has been specified with the proper value for every workbook so they can be linked to corresponding external link. |
### Remarks
If corresponding external link cannot be found for one workbook, then this workbook will be ignored. So when you set a formula later with one new external link which you intend to make the ignored workbook be linked to it, the link cannot be performed until you call this this method again with those workbooks.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class WorkbookMethodUpdateLinkedDataSourceWithWorkbookDemo
{
public static void Run()
{
// Create a main workbook with external references
Workbook mainWorkbook = new Workbook();
Worksheet mainSheet = mainWorkbook.Worksheets[0];
mainSheet.Cells["A1"].Formula = "=[ExternalWorkbook.xlsx]Sheet1!A1";
// Create external workbook that will be linked
Workbook externalWorkbook = new Workbook();
Worksheet externalSheet = externalWorkbook.Worksheets[0];
externalSheet.Cells["A1"].Value = "Updated External Value";
try
{
// Call UpdateLinkedDataSource with the external workbook array
mainWorkbook.UpdateLinkedDataSource(new Workbook[] { externalWorkbook });
// Calculate formulas to update the reference
mainWorkbook.CalculateFormula();
// Display the updated value
Console.WriteLine("Updated value in main workbook: " + mainSheet.Cells["A1"].Value);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing UpdateLinkedDataSource method: {ex.Message}");
}
// Save the result
mainWorkbook.Save("UpdateLinkedDataSourceDemo.xlsx");
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
