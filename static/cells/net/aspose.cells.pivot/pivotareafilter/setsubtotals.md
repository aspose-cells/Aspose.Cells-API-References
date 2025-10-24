##PivotAreaFilter.SetSubtotals
PivotAreaFilter method. Subtotal for the filter
## PivotAreaFilter.SetSubtotals method
Subtotal for the filter.
```csharp
public void SetSubtotals(PivotFieldSubtotalType subtotalType, bool shown)
```
| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | The subtotal function. |
| shown | Boolean | Indicates if showing this subtotal data. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotAreaFilterMethodSetSubtotalsWithPivotFieldSubtotalTypeBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data for pivot table
Cells cells = worksheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 5;
cells["A4"].Value = "Banana";
cells["B4"].Value = 7;
cells["A5"].Value = "Apple";
cells["B5"].Value = 8;
// Create pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("=A1:B5", "C3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Create a pivot area with the pivot table parameter
PivotArea pivotArea = new PivotArea(pivotTable);
PivotAreaFilter filter = new PivotAreaFilter();
try
{
// Call SetSubtotals with Sum subtotal type and set to show
filter.SetSubtotals(PivotFieldSubtotalType.Sum, true);
// Verify if subtotal is set
bool isSumSet = filter.IsSubtotalSet(PivotFieldSubtotalType.Sum);
Console.WriteLine($"Sum subtotal is set: {isSumSet}");
// Refresh pivot table to see changes
pivotTable.RefreshData();
pivotTable.CalculateData();
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetSubtotals method: {ex.Message}");
}
// Save the result
workbook.Save("PivotAreaFilterSetSubtotalsDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
