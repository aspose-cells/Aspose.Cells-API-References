##Shape.LeftCM
Shape property. Represents the horizontal offset of shape from its left column in unit of centimeters
## Shape.LeftCM property
Represents the horizontal offset of shape from its left column, in unit of centimeters.
```csharp
public double LeftCM { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyLeftCMDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
// Set and get LeftCM property
shape.LeftCM = 3.0;
Console.WriteLine("Shape left position (cm): " + shape.LeftCM);
// Modify left position if it's 3 cm
if (shape.LeftCM == 3.0)
{
shape.LeftCM = 1.0;
Console.WriteLine("Adjusted shape left position (cm): " + shape.LeftCM);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
