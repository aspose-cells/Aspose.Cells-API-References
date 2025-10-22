##Class CustomGeometry
Aspose.Cells.Drawing.CustomGeometry class. Represents a custom geometric shape
## CustomGeometry class
Represents a custom geometric shape.
```csharp
public class CustomGeometry : Geometry
```
## Properties
| Name | Description |
| --- | --- |
| [Paths](../../aspose.cells.drawing/customgeometry/paths/) { get; } | Gets path collection information when shape is a NotPrimitive autoshape |
| [ShapeAdjustValues](../../aspose.cells.drawing/geometry/shapeadjustvalues/) { get; } | Gets a collection of shape adjust value(Inherited from [`Geometry`](../geometry/).) |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class DrawingClassCustomGeometryDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a NotPrimitive autoshape with correct parameters
Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 0, 0, 0, 0, 200, 300);
// Get the CustomGeometry instance from the shape
CustomGeometry customGeometry = shape.Geometry as CustomGeometry;
// Create a new path in the geometry's path collection
int pathIndex = customGeometry.Paths.Add();
ShapePath path = customGeometry.Paths[pathIndex];
// Add path segments using direct method calls
path.MoveTo(0, 0);
path.LineTo(1000, 0);
path.LineTo(1000, 1000);
path.LineTo(0, 1000);
path.Close();
// Save the workbook
workbook.Save("CustomGeometryDemo.xlsx");
}
}
}
```
### See Also
* class [Geometry](../geometry/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
