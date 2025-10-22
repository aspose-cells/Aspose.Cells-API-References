##Shape.Y
Shape property. Gets and sets the vertical offset of shape from worksheet top borderin unit of pixels
## Shape.Y property
Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels.
```csharp
public int Y { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyYDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
// Set and demonstrate the Y property
shape.Y = 200;
Console.WriteLine("Shape Y position: " + shape.Y);
// Modify Y position based on condition
if (shape.Y == 200)
shape.Y = 100;
Console.WriteLine("Updated Shape Y position: " + shape.Y);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
