##ListColumn.GetCustomTotalsRowFormula
ListColumn method. Gets the formula of totals row of this list column
## ListColumn.GetCustomTotalsRowFormula method
Gets the formula of totals row of this list column.
```csharp
public string GetCustomTotalsRowFormula(bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |
### Return Value
The formula of this list column.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListColumnMethodGetCustomTotalsRowFormulaWithBooleanBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Column1");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(20);
// Create a list object
int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
ListObject listObject = worksheet.ListObjects[index];
// Set custom totals formula
ListColumn listColumn = listObject.ListColumns[0];
listColumn.TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Custom;
listColumn.SetCustomTotalsRowFormula("=SUM([Column1])", false, false);
// Get and display the custom totals formula
string formula = listColumn.GetCustomTotalsRowFormula(false, true);
Console.WriteLine("Custom Totals Formula: " + formula);
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
