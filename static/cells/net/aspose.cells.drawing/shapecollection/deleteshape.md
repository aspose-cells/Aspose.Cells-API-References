##ShapeCollection.DeleteShape
ShapeCollection method. Delete a shape. If the shape is in the group or is a comment shape it will not be deleted
## ShapeCollection.DeleteShape method
Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted.
```csharp
public void DeleteShape(Shape shape)
```
| Parameter | Type | Description |
| --- | --- | --- |
| shape | Shape |  |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapeCollectionMethodDeleteShapeWithShapeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the shapes collection
ShapeCollection shapes = worksheet.Shapes;
// Add first rectangle shape
Shape firstShape = shapes.AddRectangle(2, 0, 2, 0, 50, 50);
// Add second rectangle shape
Shape secondShape = shapes.AddRectangle(6, 0, 2, 0, 30, 30);
// Delete the first shape
shapes.DeleteShape(firstShape);
// Save the workbook
workbook.Save("DeleteShapeDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
