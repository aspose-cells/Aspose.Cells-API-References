##Enum PivotTableSelectionType
Aspose.Cells.Pivot.PivotTableSelectionType enum. Specifies what can be selected in a PivotTable during a structured selection. These constants can be combined to select multiple types
## PivotTableSelectionType enumeration
Specifies what can be selected in a PivotTable during a structured selection. These constants can be combined to select multiple types.
```csharp
public enum PivotTableSelectionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| DataAndLabel | `0` | Data and labels |
| DataOnly | `2` | Only selects data |
| LabelOnly | `1` | Only selects labels |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableSelectionTypeDemo
{
public static void PivotTableSelectionTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data for the PivotTable
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(150);
worksheet.Cells["A4"].PutValue("A");
worksheet.Cells["B4"].PutValue(200);
worksheet.Cells["A5"].PutValue("B");
worksheet.Cells["B5"].PutValue(250);
// Create a PivotTable
int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to the PivotTable
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Create a PivotArea and set its properties
PivotArea pivotArea = new PivotArea(pivotTable);
pivotArea.AxisType = PivotFieldType.Row;
pivotArea.OnlyData = false;
pivotArea.OnlyLabel = true;
pivotArea.IsRowGrandIncluded = true;
pivotArea.IsColumnGrandIncluded = true;
pivotArea.IsOutline = false;
// Select the area with specific selection type
pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);
// Save the workbook
workbook.Save("PivotTableSelectionTypeExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
