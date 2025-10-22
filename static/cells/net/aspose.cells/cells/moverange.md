##Cells.MoveRange
Cells method. Moves the range
## Cells.MoveRange method
Moves the range.
```csharp
public void MoveRange(CellArea sourceArea, int destRow, int destColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceArea | CellArea | The range which should be moved. |
| destRow | Int32 | The dest row. |
| destColumn | Int32 | The dest column. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodMoveRangeWithCellAreaInt32Int32Demo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Put values in cells
cells["A1"].PutValue("Original");
cells["B1"].PutValue(100);
cells["A2"].PutValue("Data");
cells["B2"].PutValue(200);
// Define the cell area to move (A1:B2)
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 1;
area.EndColumn = 1;
// Move the range down by 2 rows and right by 3 columns
cells.MoveRange(area, 2, 3);
// Save the workbook
workbook.Save("MoveRangeExample.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
