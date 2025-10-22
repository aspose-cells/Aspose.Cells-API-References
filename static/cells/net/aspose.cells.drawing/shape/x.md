##Shape.X
Shape property. Gets and sets the horizontal offset of shape from worksheet left borderin unit of pixels
## Shape.X property
Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels.
```csharp
public int X { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyXDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
// Set initial X position
shape.X = 200;
Console.WriteLine("Initial X position: " + shape.X);
// Modify X position if it equals 3 (demonstrating the test case logic)
if (shape.X == 3)
{
shape.X = 1;
}
else
{
// For demonstration, change X position to 300
shape.X = 300;
}
Console.WriteLine("Final X position: " + shape.X);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
