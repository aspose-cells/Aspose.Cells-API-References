##ShapeSegmentPathCollection.Add
ShapeSegmentPathCollection method. Add a segment path in creation path
## ShapeSegmentPathCollection.Add method
Add a segment path in creation path.
```csharp
public int Add(ShapePathType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | ShapePathType | The path type. |
### Return Value
Returns the position of [`ShapeSegmentPath`](../../shapesegmentpath/) object in the list.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ShapeSegmentPathCollectionMethodAddWithShapePathTypeDemo
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
ShapeSegmentPathCollection segmentList = path.PathSegementList;
segmentList.Add(ShapePathType.Close);
// Display the count of path segments
Console.WriteLine("Number of path segments: " + segmentList.Count);
// Iterate through each segment and display its type
foreach (ShapeSegmentPath segment in segmentList)
{
Console.WriteLine("Segment type: " + segment.Type);
}
//add free form
worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { path });
// Save the workbook to observe the shape modifications
workbook.Save("ShapeSegmentPathCollectionAddDemo.xlsx");
}
}
}
```
### See Also
* enum [ShapePathType](../../shapepathtype/)
* class [ShapeSegmentPathCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
