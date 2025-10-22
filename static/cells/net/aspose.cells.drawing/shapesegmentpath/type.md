##ShapeSegmentPath.Type
ShapeSegmentPath property. Gets the path segment type
## ShapeSegmentPath.Type property
Gets the path segment type
```csharp
public ShapePathType Type { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ShapeSegmentPathPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
try
{
//Create a new shape path
ShapePath shapePath = new ShapePath();
// Move to starting point
shapePath.MoveTo(10, 10);
// Call LineTo method with (Single, Single) parameters
shapePath.LineTo(50.5f, 10.5f);
shapePath.LineTo(50.5f, 50.5f);
shapePath.LineTo(10.5f, 50.5f);
shapePath.Close();
// Access the PathSegementList property
ShapeSegmentPathCollection segmentList = shapePath.PathSegementList;
// Display the count of path segments
Console.WriteLine("Number of path segments: " + segmentList.Count);
// Iterate through each segment and display its type
foreach (ShapeSegmentPath segment in segmentList)
{
Console.WriteLine("Segment type: " + segment.Type);
}
//add free form
worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });
}
catch (Exception ex)
{
Console.WriteLine($"Error executing LineTo method: {ex.Message}");
}
// Save the workbook
workbook.Save("ShapeSegmentPathTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [ShapePathType](../../shapepathtype/)
* class [ShapeSegmentPath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
