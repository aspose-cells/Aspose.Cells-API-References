##Class ShapeSegmentPath
Aspose.Cells.Drawing.ShapeSegmentPath class. Represents a segment path in a path of the freeform
## ShapeSegmentPath class
Represents a segment path in a path of the freeform.
```csharp
public class ShapeSegmentPath
```
## Properties
| Name | Description |
| --- | --- |
| [Points](../../aspose.cells.drawing/shapesegmentpath/points/) { get; } | Gets the points in path segment |
| [Type](../../aspose.cells.drawing/shapesegmentpath/type/) { get; } | Gets the path segment type |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class DrawingClassShapeSegmentPathDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a freeform shape to the worksheet
Shape shape = worksheet.Shapes.AddFreeform(0, 0, 0, 0, 200, 200, new ShapePath[] { new ShapePath() });
// Get the geometry path of the shape
CustomGeometry geometry = shape.Geometry as CustomGeometry;
ShapePath shapePath = geometry.Paths[0];
// Access the first segment path (if exists)
if (shapePath.PathSegementList.Count > 0)
{
ShapeSegmentPath segmentPath = shapePath.PathSegementList[0];
// Demonstrate properties of ShapeSegmentPath
Console.WriteLine("Segment Path Type: " + segmentPath.Type);
Console.WriteLine("Number of Points: " + segmentPath.Points.Count);
// Iterate through points in the segment path
foreach (ShapePathPoint point in segmentPath.Points)
{
Console.WriteLine($"Point coordinates: X={point.X}, Y={point.Y}");
}
}
// Save the workbook
workbook.Save("ShapeSegmentPathDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
