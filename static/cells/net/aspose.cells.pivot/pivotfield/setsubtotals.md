##PivotField.SetSubtotals
PivotField method. Sets whether the specified field shows that subtotals
## PivotField.SetSubtotals method
Sets whether the specified field shows that subtotals.
```csharp
public void SetSubtotals(PivotFieldSubtotalType subtotalType, bool shown)
```
| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | subtotals type. |
| shown | Boolean | whether the specified field shows that subtotals. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldMethodSetSubtotalsWithPivotFieldSubtotalTypeBooleanDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
var cells = sheet.Cells;
cells["A1"].Value = "Category";
cells["B1"].Value = "Product";
cells["C1"].Value = "Sales";
cells["A2"].Value = "Electronics";
cells["B2"].Value = "TV";
cells["C2"].Value = 1000;
cells["A3"].Value = "Electronics";
cells["B3"].Value = "Radio";
cells["C3"].Value = 500;
cells["A4"].Value = "Clothing";
cells["B4"].Value = "Shirt";
cells["C4"].Value = 300;
cells["A5"].Value = "Clothing";
cells["B5"].Value = "Pants";
cells["C5"].Value = 400;
// Add pivot table
int pivotIndex = sheet.PivotTables.Add("=A1:C5", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[pivotIndex];
// Add row fields
int rowIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
PivotField rowField = pivotTable.RowFields[rowIndex];
// Demonstrate SetSubtotals with PivotFieldSubtotalType and boolean
rowField.SetSubtotals(PivotFieldSubtotalType.Sum, true);
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Refresh and calculate pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotFieldSetSubtotalsDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
