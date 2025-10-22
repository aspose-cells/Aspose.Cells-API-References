##PivotArea.OnlyLabel
PivotArea property. Indicates whether only the data labels for an item selection are selected
## PivotArea.OnlyLabel property
Indicates whether only the data labels for an item selection are selected.
```csharp
public bool OnlyLabel { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotAreaPropertyOnlyLabelDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Configure pivot area
PivotArea pivotArea = new PivotArea(pivotTable);
pivotArea.AxisType = PivotFieldType.Row;
pivotArea.OnlyLabel = true; // Key property demonstration
// Apply selection
pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);
workbook.Save("PivotAreaOnlyLabelDemo.xlsx");
}
}
}
```
### See Also
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
