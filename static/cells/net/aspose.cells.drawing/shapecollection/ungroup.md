##ShapeCollection.Ungroup
ShapeCollection method. Ungroups the shape items
## ShapeCollection.Ungroup method
Ungroups the shape items.
```csharp
public void Ungroup(GroupShape group)
```
| Parameter | Type | Description |
| --- | --- | --- |
| group | GroupShape | The group shape. |
### Remarks
If the group shape is grouped by another group shape,nothing will be done.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodUngroupWithGroupShapeDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the shapes collection
ShapeCollection shapes = worksheet.Shapes;
// Add first rectangle shape
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
// Add second rectangle shape
shapes.AddRectangle(6, 0, 2, 0, 30, 30);
// Create array of shapes to group
Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };
// Group the shapes
GroupShape groupShape = shapes.Group(shapesArr);
// Ungroup the group shape
shapes.Ungroup(groupShape);
}
}
}
```
### See Also
* class [GroupShape](../../groupshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
