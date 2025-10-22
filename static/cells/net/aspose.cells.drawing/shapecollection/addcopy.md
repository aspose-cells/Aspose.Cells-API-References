##ShapeCollection.AddCopy
ShapeCollection method. Adds and copy a shape to the worksheet
## ShapeCollection.AddCopy method
Adds and copy a shape to the worksheet.
```csharp
public Shape AddCopy(Shape sourceShape, int topRow, int top, int leftColumn, int left)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceShape | Shape | Source shape. |
| topRow | Int32 | The top row index. |
| top | Int32 | Represents the vertical offset from its top row, in unit of pixel. |
| leftColumn | Int32 | The left column index. |
| left | Int32 | Represents the horizontal offset from its left column, in unit of pixel. |
### Return Value
The new [`Shape`](../../shape/) object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodAddCopyWithShapeInt32Int32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the shapes collection
ShapeCollection shapes = worksheet.Shapes;
// Add a rectangle shape
RectangleShape rectangle = shapes.AddRectangle(2, 0, 2, 0, 130, 130);
// Add a copy of the rectangle shape with new position
shapes.AddCopy(rectangle, 7, 0, 7, 0);
// Save the workbook
workbook.Save("ShapeCollectionMethodAddCopyDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
