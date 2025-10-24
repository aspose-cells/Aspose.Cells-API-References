##ShapeSegmentPathCollection.Item
ShapeSegmentPathCollection property. Gets ShapeSegmentPath object
## ShapeSegmentPathCollection indexer
Gets [`ShapeSegmentPath`](../../shapesegmentpath/) object.
```csharp
public ShapeSegmentPath this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Return Value
Returns a [`ShapeSegmentPath`](../../shapesegmentpath/) object.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ShapeSegmentPathCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ShapePath path = new ShapePath();
// Start a new path
path.MoveTo(10, 10);
// Draw a line segment
path.LineTo(100, 100);
// Access the PathSegementList property
ShapeSegmentPathCollection segmentPaths = path.PathSegementList;
segmentPaths.Add(ShapePathType.Close);
// Display the count of path segments
Console.WriteLine("Number of path segments: " + segmentPaths.Count);
// Demonstrate reading the Item property
for (int i = 0; i < segmentPaths.Count; i++)
{
ShapeSegmentPath segment = segmentPaths[i];
Console.WriteLine($"Segment {i} type: {segment.Type}");
}
//add free form
worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });
// Save the workbook
workbook.Save("ShapeSegmentPathCollectionPropertyItemDemo.xlsx");
}
}
}
```
### See Also
* class [ShapeSegmentPath](../../shapesegmentpath/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
