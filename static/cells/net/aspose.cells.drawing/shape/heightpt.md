##Shape.HeightPt
Shape property. Represents the height of the shape in unit of points
## Shape.HeightPt property
Represents the height of the shape, in unit of points.
```csharp
public double HeightPt { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyHeightPtDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 100);
// Set and get HeightPt property
shape.HeightPt = 50;
Console.WriteLine("Shape height in points: " + shape.HeightPt);
// Modify height if it matches a condition
if (shape.HeightPt == 50)
{
shape.HeightPt = 30;
Console.WriteLine("Modified shape height: " + shape.HeightPt);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
