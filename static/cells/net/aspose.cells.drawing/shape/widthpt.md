##Shape.WidthPt
Shape property. Represents the width of the shape in unit of point
## Shape.WidthPt property
Represents the width of the shape, in unit of point.
```csharp
public double WidthPt { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyWidthPtDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
// Set and get the width in points
shape.WidthPt = 150;
Console.WriteLine("Shape width in points: " + shape.WidthPt);
// Modify width if condition is met
if (shape.WidthPt == 150)
{
shape.WidthPt = 100;
Console.WriteLine("Modified shape width in points: " + shape.WidthPt);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
