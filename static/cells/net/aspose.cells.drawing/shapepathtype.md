##Enum ShapePathType
Aspose.Cells.Drawing.ShapePathType enum. Represents path segment type
## ShapePathType enumeration
Represents path segment type.
```csharp
public enum ShapePathType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| LineTo | `1` | Straight line segment |
| CubicBezierCurveTo | `3` | Cubic Bezier curve |
| MoveTo | `0` | Start a new path |
| Close | `128` | If the starting POINT and the end POINT are not the same, a single straight line is drawn to connect the starting POINT and ending POINT of the path. |
| End | `4` | The end of the current path |
| Escape | `5` | Escape |
| ArcTo | `6` | An arc |
| Unknown | `7` | Unknown |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class DrawingClassShapePathTypeDemo
{
public static void Run()
{
// Create a new workbook for demonstration
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
try
{
// Create a shape to demonstrate path types
Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 10, 10, 200, 200);
// Create a custom geometry path
Geometry geometry = shape.Geometry;
ShapePath path = new ShapePath();
// Demonstrate different ShapePathType values
Console.WriteLine("Available ShapePathType values:");
Console.WriteLine($"LineTo: {ShapePathType.LineTo}");
Console.WriteLine($"CubicBezierCurveTo: {ShapePathType.CubicBezierCurveTo}");
Console.WriteLine($"MoveTo: {ShapePathType.MoveTo}");
Console.WriteLine($"Close: {ShapePathType.Close}");
Console.WriteLine($"End: {ShapePathType.End}");
// Apply some path operations
path.MoveTo(10, 10);
path.LineTo(100, 100);
path.Close();
// Save the workbook
workbook.Save("ShapePathTypeDemo.xlsx");
Console.WriteLine("Demo completed successfully");
}
catch (Exception ex)
{
Console.WriteLine($"Error working with ShapePathType: {ex.Message}");
}
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
