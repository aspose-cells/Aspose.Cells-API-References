##Shape.Width
Shape property. Represents the width of shape in unit of pixels
## Shape.Width property
Represents the width of shape, in unit of pixels.
```csharp
public int Width { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with correct parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 50);
// Set initial width and display it
shape.Width = 300;
Console.WriteLine("Initial width: " + shape.Width);
// Modify width based on condition
if (shape.Width == 300)
shape.Width = 150;
Console.WriteLine("Modified width: " + shape.Width);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
