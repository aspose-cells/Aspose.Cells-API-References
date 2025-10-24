##PivotItem.Move
PivotItem method. Moves the item up or down
## PivotItem.Move method
Moves the item up or down
```csharp
public void Move(int count, bool isSameParent)
```
| Parameter | Type | Description |
| --- | --- | --- |
| count | Int32 | The number of moving up or down. Move the item up if this is less than zero; Move the item down if this is greater than zero. |
| isSameParent | Boolean | Specifying whether moving operation is in the same parent node or not |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotItemMethodMoveWithInt32BooleanDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Create sample data for pivot table
sheet.Cells["A1"].PutValue("Product");
sheet.Cells["A2"].PutValue("A");
sheet.Cells["A3"].PutValue("B");
sheet.Cells["A4"].PutValue("C");
sheet.Cells["B1"].PutValue("Sales");
sheet.Cells["B2"].PutValue(100);
sheet.Cells["B3"].PutValue(200);
sheet.Cells["B4"].PutValue(300);
// Add pivot table
int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
// Get pivot items and demonstrate Move method
PivotItemCollection items = pivotTable.RowFields[0].PivotItems;
// Move first item to position 1 (second position) with child items
items[0].Move(1, true);
// Save the workbook
wb.Save("PivotItemMoveDemo.xlsx");
}
}
}
```
### See Also
* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
