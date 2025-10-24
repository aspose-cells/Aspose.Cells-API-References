##ShapeCollection.Remove
ShapeCollection method. Remove the shape
## ShapeCollection.Remove method
Remove the shape.
```csharp
public void Remove(Shape shape)
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
public class ShapeCollectionMethodRemoveWithShapeDemo
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
// Get the first shape by name or index
Shape shapeToRemove = shapes["Rectangle 1"]; // or shapes[0];
if (shapeToRemove != null)
{
// Remove the shape from the collection
shapes.Remove(shapeToRemove);
}
// Save the workbook
workbook.Save("ShapeRemoveDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
