##ShapeCollection.Group
ShapeCollection method. Group the shapes
## ShapeCollection.Group method
Group the shapes.
```csharp
public GroupShape Group(Shape[] groupItems)
```
| Parameter | Type | Description |
| --- | --- | --- |
| groupItems | Shape[] | the group items. |
### Return Value
Return the group shape.
### Remarks
The shape in the groupItems should not be grouped. The shape must be in this Shapes collection.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodGroupWithShapeArrayDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the shapes collection
ShapeCollection shapes = worksheet.Shapes;
// Add first rectangle shape
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
// Add second rectangle shape
shapes.AddRectangle(6, 0, 2, 0, 30, 30);
// Create array with the shapes to group
Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };
// Group the shapes
GroupShape groupShape = shapes.Group(shapesArr);
// Save the workbook
workbook.Save("GroupShapesDemo.xlsx");
}
}
}
```
### See Also
* class [GroupShape](../../groupshape/)
* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
