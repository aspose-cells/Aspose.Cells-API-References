##ListColumn.SetCustomTotalsRowFormula
ListColumn method. Gets the formula of totals row of this list column
## ListColumn.SetCustomTotalsRowFormula method
Gets the formula of totals row of this list column.
```csharp
public void SetCustomTotalsRowFormula(string formula, bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | the formula for this list column. |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListColumnMethodSetCustomTotalsRowFormulaWithStringBooleanBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Column1");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(20);
// Create a list object
int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
ListObject listObject = worksheet.ListObjects[index];
// Enable totals row and set custom formula
listObject.ShowTotals = true;
listObject.ListColumns[0].TotalsCalculation = TotalsCalculation.Custom;
listObject.ListColumns[0].SetCustomTotalsRowFormula("=SUM([Column1])", false, false);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
