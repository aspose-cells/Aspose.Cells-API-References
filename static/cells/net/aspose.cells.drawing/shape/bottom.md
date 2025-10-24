##Shape.Bottom
Shape property. Represents the width of the shapes vertical offset from its lower bottom corner row in unit of pixels
## Shape.Bottom property
Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels.
```csharp
public int Bottom { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyBottomDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
// Set initial position
shape.Top = 200;
shape.Left = 200;
// Demonstrate Bottom property
Console.WriteLine("Original Bottom position: " + shape.Bottom);
// Modify Bottom position
if (shape.Bottom == 300)  // 200 (Top) + 100 (Height)
{
shape.Bottom = 250;  // This will change the Top position (250 - 100 = 150)
Console.WriteLine("New Bottom position: " + shape.Bottom);
Console.WriteLine("New Top position: " + shape.Top);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
