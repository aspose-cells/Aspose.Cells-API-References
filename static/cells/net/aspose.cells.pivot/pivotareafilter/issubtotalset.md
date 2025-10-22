##PivotAreaFilter.IsSubtotalSet
PivotAreaFilter method. Gets which subtotal is set for this filter
## PivotAreaFilter.IsSubtotalSet method
Gets which subtotal is set for this filter.
```csharp
public bool IsSubtotalSet(PivotFieldSubtotalType subtotalType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | The subtotal function type. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotAreaFilterMethodIsSubtotalSetWithPivotFieldSubtotalTypeDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("A");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field and configure subtotals
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
PivotField rowField = pivotTable.RowFields["Category"];
rowField.IsAutoSubtotals = true;
rowField.SetSubtotals(PivotFieldSubtotalType.Automatic, true);
// Create pivot area and check subtotal setting
PivotArea pivotArea = new PivotArea(pivotTable);
pivotArea.SelectField(PivotFieldType.Row, "Category");
// Demonstrate IsSubtotalSet usage
bool isSubtotalSet = pivotArea.Filters[0].IsSubtotalSet(PivotFieldSubtotalType.Automatic);
Console.WriteLine($"Is Automatic subtotal set: {isSubtotalSet}");
// Save the workbook
workbook.Save("PivotSubtotalDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
