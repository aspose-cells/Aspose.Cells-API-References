##Shape.Geometry
Shape property. Gets the geometry
## Shape.Geometry property
Gets the geometry
```csharp
public Geometry Geometry { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyGeometryDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with correct parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
// Check geometry properties
if (shape.Geometry != null)
{
Console.WriteLine("Shape has geometry path with " + shape.Geometry.ShapeAdjustValues.Count + " adjustment points");
// Add an adjustment point (demonstrating geometry modification)
shape.Geometry.ShapeAdjustValues.Add("adj1", 0.5);
Console.WriteLine("Added adjustment point. Total now: " + shape.Geometry.ShapeAdjustValues.Count);
}
// Save the workbook
workbook.Save("ShapeGeometryDemo.xlsx");
}
}
}
```
### See Also
* class [Geometry](../../geometry/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
