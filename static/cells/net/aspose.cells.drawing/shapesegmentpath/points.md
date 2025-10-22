##ShapeSegmentPath.Points
ShapeSegmentPath property. Gets the points in path segment
## ShapeSegmentPath.Points property
Gets the points in path segment
```csharp
public ShapePathPointCollection Points { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ShapeSegmentPathPropertyPointsDemo
{
public static void Run()
{// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ShapePath path = new ShapePath();
// Start a new path
path.MoveTo(10, 10);
// Draw a line segment
path.LineTo(100, 100);
// Access the PathSegementList property
ShapeSegmentPathCollection segmentPaths = path.PathSegementList;
// Access the first segment path
ShapeSegmentPath segmentPath = segmentPaths[1];
// Display points information
Console.WriteLine("Number of points in segment: " + segmentPath.Points.Count);
Console.WriteLine("Point coordinates:");
foreach (ShapePathPoint point in segmentPath.Points)
{
Console.WriteLine($"X: {point.X}, Y: {point.Y}");
}
//add free form
worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });
// Save the workbook
workbook.Save("ShapeSegmentPathPointsDemo.xlsx");
}
}
}
```
### See Also
* class [ShapePathPointCollection](../../shapepathpointcollection/)
* class [ShapeSegmentPath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
