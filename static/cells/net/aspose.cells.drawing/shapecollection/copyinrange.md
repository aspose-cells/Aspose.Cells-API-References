##ShapeCollection.CopyInRange
ShapeCollection method. Copy shapes in the range to destination range
## ShapeCollection.CopyInRange method
Copy shapes in the range to destination range.
```csharp
public void CopyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn,
bool isContained)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceShapes | ShapeCollection | Source shapes. |
| ca | CellArea | The source range. |
| destRow | Int32 | The dest row index of the dest range. |
| destColumn | Int32 | The dest column of the dest range. |
| isContained | Boolean | Whether only copy the shapes which are contained in the range. If true,only copies the shapes in the range. Otherwise,it works as MS Office. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodCopyInRangeWithShapeCollectionCellAreaInt32InDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the shapes collection
ShapeCollection shapes = worksheet.Shapes;
// Add a rectangle shape
shapes.AddRectangle(2, 0, 2, 0, 130, 130);
// Define the cell area to copy from
CellArea area2 = new CellArea();
area2.StartColumn = 1;
area2.StartRow = 1;
area2.EndColumn = 5;
area2.EndRow = 11;
// Copy shapes within the specified range
shapes.CopyInRange(shapes, area2, 12, 1, false);
// Save the workbook
workbook.Save("ShapeCopyDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
