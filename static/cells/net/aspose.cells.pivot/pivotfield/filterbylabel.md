##PivotField.FilterByLabel
PivotField method. Filters by captions of row or column pivot field
## PivotField.FilterByLabel method
Filters by captions of row or column pivot field.
```csharp
public PivotFilter FilterByLabel(PivotFilterType type, string label1, string label2)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | PivotFilterType | The type of filtering data. |
| label1 | String | The label of filter condition |
| label2 | String | The upper-bound label of between filter condition |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldMethodFilterByLabelWithPivotFilterTypeStringStringDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["A2"].PutValue("A");
sheet.Cells["A3"].PutValue("B");
sheet.Cells["A4"].PutValue("");
sheet.Cells["A5"].PutValue("C");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["B3"].PutValue(20);
sheet.Cells["B4"].PutValue(30);
sheet.Cells["B5"].PutValue(40);
// Create pivot table with correct parameters
int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
PivotTable pivot = sheet.PivotTables[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "Category");
pivot.AddFieldToArea(PivotFieldType.Data, "Value");
// Get the pivot field
PivotField field = pivot.RowFields[0];
// Apply filters
field.FilterByLabel(PivotFilterType.CaptionNotEqual, "(blank)", "");
pivot.RefreshData();
pivot.CalculateData();
// Save the workbook
workbook.Save("PivotFilterByLabelDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
