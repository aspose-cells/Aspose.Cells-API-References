##CustomGeometry.Paths
CustomGeometry property. Gets path collection information when shape is a NotPrimitive autoshape
## CustomGeometry.Paths property
Gets path collection information when shape is a NotPrimitive autoshape
```csharp
public ShapePathCollection Paths { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class CustomGeometryPropertyPathsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a custom shape with non-primitive geometry (fixed parameters)
var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 0, 0, 10, 10, 400, 400);
// Access custom geometry through explicit cast
CustomGeometry geometry = (CustomGeometry)shape.Geometry;
// Get paths collection
ShapePathCollection paths = geometry.Paths;
Console.WriteLine($"Initial path count: {paths.Count}");
// Create a new shape path using drawing commands
paths.Add(); // Creates a new path in the collection
ShapePath newPath = paths[paths.Count - 1];
newPath.MoveTo(0, 0);
newPath.LineTo(10000, 0);
newPath.LineTo(10000, 10000);
newPath.LineTo(0, 10000);
newPath.Close();
// No explicit Add needed since path was created in the collection
Console.WriteLine($"New path count after modification: {paths.Count}");
// Save to demonstrate persistent changes
workbook.Save("CustomGeometryPathsDemo.xlsx");
}
}
}
```
### See Also
* class [ShapePathCollection](../../shapepathcollection/)
* class [CustomGeometry](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
