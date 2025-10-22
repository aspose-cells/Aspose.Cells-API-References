##Shape.Height
Shape property. Represents the height of shape in unit of pixel
## Shape.Height property
Represents the height of shape, in unit of pixel.
```csharp
public int Height { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyHeightDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);
// Set initial height
shape.Height = 150;
Console.WriteLine("Initial height: " + shape.Height);
// Modify height conditionally
if (shape.Height == 150)
{
shape.Height = 100;
Console.WriteLine("Modified height: " + shape.Height);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
