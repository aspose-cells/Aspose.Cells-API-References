##Shape.LeftToCorner
Shape property. Gets and sets the horizonal offset of shape from worksheet left border
## Shape.LeftToCorner property
Gets and sets the horizonal offset of shape from worksheet left border.
```csharp
public int LeftToCorner { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyLeftToCornerDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with correct parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);
// Set and demonstrate LeftToCorner property
shape.LeftToCorner = 50;
Console.WriteLine("Shape LeftToCorner value: " + shape.LeftToCorner);
// Modify LeftToCorner if it equals a specific value
if (shape.LeftToCorner == 50)
{
shape.LeftToCorner = 30;
Console.WriteLine("Modified LeftToCorner value: " + shape.LeftToCorner);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
