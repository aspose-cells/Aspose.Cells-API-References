##PivotArea.Select
PivotArea method. Select the area with filters
## PivotArea.Select method
Select the area with filters.
```csharp
public void Select(PivotFieldType axisType, int fieldPosition,
PivotTableSelectionType selectionType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | PivotFieldType | The region of the PivotTable to which this rule applies. |
| fieldPosition | Int32 | Position of the field within the axis to which this rule applies. |
| selectionType | PivotTableSelectionType | Specifies what can be selected in a PivotTable during a structured selection. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotAreaMethodSelectWithPivotFieldTypeInt32PivotTableSDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
PivotArea pivotArea = new PivotArea(pivotTable);
pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);
workbook.Save("PivotAreaSelectDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldType](../../pivotfieldtype/)
* enum [PivotTableSelectionType](../../pivottableselectiontype/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
