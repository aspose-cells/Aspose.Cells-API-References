##Shape.TopToCorner
Shape property. Gets and sets the vertical offset of shape from worksheet top border in unit of pixels
## Shape.TopToCorner property
Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels.
```csharp
public int TopToCorner { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyTopToCornerDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);
// Set and display the TopToCorner property
shape.TopToCorner = 50;
Console.WriteLine("Shape TopToCorner: " + shape.TopToCorner);
// Modify the TopToCorner property
if (shape.TopToCorner == 50)
{
shape.TopToCorner = 20;
Console.WriteLine("Updated Shape TopToCorner: " + shape.TopToCorner);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
