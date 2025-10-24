##Shape.Right
Shape property. Represents the width of the shapes horizontal offset from its lower right corner column in unit of pixels
## Shape.Right property
Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels.
```csharp
public int Right { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyRightDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet
Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
// Set and get the Right property
shape.Right = 200;
Console.WriteLine("Shape Right position: " + shape.Right);
// Modify the Right property conditionally
if (shape.Right == 200)
shape.Right = 150;
Console.WriteLine("Modified Shape Right position: " + shape.Right);
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
