##Class Geometry
Aspose.Cells.Drawing.Geometry class. Represents a geometric shape
## Geometry class
Represents a geometric shape.
```csharp
public abstract class Geometry
```
## Properties
| Name | Description |
| --- | --- |
| [ShapeAdjustValues](../../aspose.cells.drawing/geometry/shapeadjustvalues/) { get; } | Gets a collection of shape adjust value |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
public class DrawingClassGeometryDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape to the worksheet
Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);
// Access the geometry of the shape
Geometry geometry = rectangle.Geometry;
// Add shape adjustment guides directly to the collection
geometry.ShapeAdjustValues.Add("Roundness", 0.3);
geometry.ShapeAdjustValues.Add("Angle", 45.0);
// Save the modified workbook
workbook.Save("GeometryDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
