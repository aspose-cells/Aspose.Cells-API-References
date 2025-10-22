##PivotTable.ShowReportFilterPage
PivotTable method. Show all the report filter pages according to PivotField the PivotField must be located in the PageFields
## PivotTable.ShowReportFilterPage method
Show all the report filter pages according to PivotField, the PivotField must be located in the PageFields.
```csharp
public void ShowReportFilterPage(PivotField pageField)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pageField | PivotField | The PivotField object |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodShowReportFilterPageWithPivotFieldDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook("source.xlsx");
// Access first worksheet and pivot table
Worksheet worksheet = workbook.Worksheets[0];
PivotTable pivotTable = worksheet.PivotTables[0];
// Show report filter pages for each page field
foreach (PivotField pageField in pivotTable.PageFields)
{
pivotTable.ShowReportFilterPage(pageField);
}
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
