##Class ShapePath
Aspose.Cells.Drawing.ShapePath class. Represents a creation path consisting of a series of moves lines and curves that when combined will form a geometric shape
## ShapePath class
Represents a creation path consisting of a series of moves, lines and curves that when combined will form a geometric shape.
```csharp
public class ShapePath
```
## Constructors
| Name | Description |
| --- | --- |
| [ShapePath](shapepath/)() | Initializes a new instance of the `ShapePath` class. |
## Properties
| Name | Description |
| --- | --- |
| [HeightPixel](../../aspose.cells.drawing/shapepath/heightpixel/) { get; set; } | Gets the height of this path in unit of pixels. |
| [PathSegementList](../../aspose.cells.drawing/shapepath/pathsegementlist/) { get; } | Gets [`ShapeSegmentPathCollection`](../shapesegmentpathcollection/) list |
| [WidthPixel](../../aspose.cells.drawing/shapepath/widthpixel/) { get; set; } | Gets the width of this path in unit of pixels. |
## Methods
| Name | Description |
| --- | --- |
| [ArcTo](../../aspose.cells.drawing/shapepath/arcto/)(float, float, float, float) | Appends an elliptical arc to the current figure. The starting point is the end point of the current figure. |
| [Close](../../aspose.cells.drawing/shapepath/close/)() | Closes the current figure and starts a new figure. If the current figure contains a sequence of connected lines and curves, the method closes the loop by connecting a line from the endpoint to the starting point. |
| [CubicBezierTo](../../aspose.cells.drawing/shapepath/cubicbezierto/)(float, float, float, float, float, float) | Appends a cubic Bézier curve to the current figure. The starting point is the end point of the current figure.Unit: Pixel. |
| [LineTo](../../aspose.cells.drawing/shapepath/lineto/)(float, float) | Appends a line segment to the current figure. The starting point is the end point of the current figure.Unit: Pixel. |
| [MoveTo](../../aspose.cells.drawing/shapepath/moveto/)(float, float) | Starts a new figure from the specified point without closing the current figure. All subsequent points added to the path are added to this new figure.Unit: Pixel. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassShapePathDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a custom shape with all required parameters
Shape customShape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 200, 100, 0, 0);
// Access the ShapePathCollection
ShapePathCollection shapePaths = customShape.Paths;
// Add a new path and access it
int pathIndex = shapePaths.Add();
ShapePath newPath = shapePaths[pathIndex];
// Output the number of paths
Console.WriteLine("Number of paths in the ShapePathCollection: " + shapePaths.Count.ToString());
// Save the workbook
workbook.Save("ShapePathDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
