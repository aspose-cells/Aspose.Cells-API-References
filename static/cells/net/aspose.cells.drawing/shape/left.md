##Shape.Left
Shape property. Represents the horizontal offset of shape from its left column in unit of pixels
## Shape.Left property
Represents the horizontal offset of shape from its left column, in unit of pixels.
```csharp
public int Left { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyLeftDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate Left property
Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
// Set initial Left position
shape.Left = 200;
Console.WriteLine("Shape Left position: " + shape.Left);
// Modify Left position conditionally
if (shape.Left == 200)
{
shape.Left = 150;
Console.WriteLine("Adjusted Shape Left position: " + shape.Left);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
