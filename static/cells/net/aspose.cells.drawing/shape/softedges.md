##Shape.SoftEdges
Shape property. Gets and sets the radius of blur to apply to the edges in unit of points
## Shape.SoftEdges property
Gets and sets the radius of blur to apply to the edges, in unit of points.
```csharp
public double SoftEdges { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertySoftEdgesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with correct parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
// Set soft edges effect with radius of 5 points (0.5d = 5 points)
shape.SoftEdges = 0.5d;
// Save the workbook
workbook.Save("SoftEdgesDemo.xlsx");
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
