##Class ShapePathPoint
Aspose.Cells.Drawing.ShapePathPoint class. Specify position coordinates or angle markers. Position coordinates represent the coordinates of a path in a coordinate space e.g. X/Y. Angle markers indicate angular changes in a path e.g. the start and swing angles of an arc
## ShapePathPoint class
Specify position coordinates or angle markers. Position coordinates represent the coordinates of a path in a coordinate space (e.g. X/Y). Angle markers indicate angular changes in a path (e.g. the start and swing angles of an arc).
```csharp
public class ShapePathPoint
```
## Properties
| Name | Description |
| --- | --- |
| [Type](../../aspose.cells.drawing/shapepathpoint/type/) { get; } | Specifies the value type of the current object. |
| [X](../../aspose.cells.drawing/shapepathpoint/x/) { get; set; } | (**Obsolete.**) Gets and sets x coordinate for this position coordinate. Unit EMUs. |
| [XAngle](../../aspose.cells.drawing/shapepathpoint/xangle/) { get; set; } | When the object is an angle marker, get or set the first angle in degrees. |
| [XPixel](../../aspose.cells.drawing/shapepathpoint/xpixel/) { get; set; } | When the object is a position coordinate, get or set the x coordinate in pixels. |
| [Y](../../aspose.cells.drawing/shapepathpoint/y/) { get; set; } | (**Obsolete.**) Gets y coordinate for this position coordinate. Unit EMUs. |
| [YAngle](../../aspose.cells.drawing/shapepathpoint/yangle/) { get; set; } | When the object is an angle marker, get or set the second angle in degrees. |
| [YPixel](../../aspose.cells.drawing/shapepathpoint/ypixel/) { get; set; } | When the object is a position coordinate, get or set the y coordinate in pixels. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class DrawingClassShapePathPointDemo
{
public static void Run()
{
// Create a new workbook for demonstration
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
try
{
// Add a shape that will contain path points with all required parameters
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 10, 10, 200, 200);
// Get the geometry path points
CustomGeometry geometry = shape.Geometry as CustomGeometry;
if (geometry != null && geometry.Paths.Count > 0)
{
ShapePath path = geometry.Paths[0];
// Access an existing path point (if available)
if (path.PathSegementList.Count > 0)
{
// Get the first point (actual implementation may vary based on segment type)
ShapePathPoint point = path.PathSegementList[0].Points[0];
// Display the point coordinates
Console.WriteLine($"ShapePathPoint at X: {point.X}, Y: {point.Y}");
}
}
// Save the workbook
workbook.Save("ShapePathPointDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error working with ShapePathPoint: {ex.Message}");
}
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
