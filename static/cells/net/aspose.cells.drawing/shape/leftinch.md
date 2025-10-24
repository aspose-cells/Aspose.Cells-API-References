##Shape.LeftInch
Shape property. Represents the horizontal offset of shape from its left column in unit of inches
## Shape.LeftInch property
Represents the horizontal offset of shape from its left column, in unit of inches.
```csharp
public double LeftInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyLeftInchDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);
// Set and demonstrate LeftInch property
shape.LeftInch = 3;
Console.WriteLine("Shape left position (inches): " + shape.LeftInch);
// Modify left position if it's 3 inches
if (shape.LeftInch == 3)
{
shape.LeftInch = 1;
Console.WriteLine("Adjusted shape left position (inches): " + shape.LeftInch);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
