##Shape.WidthInch
Shape property. Represents the width of the shape in unit of inch
## Shape.WidthInch property
Represents the width of the shape, in unit of inch.
```csharp
public double WidthInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyWidthInchDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);
// Set width in inches
shape.WidthInch = 3;
Console.WriteLine("Shape width (inches): " + shape.WidthInch);
// Modify width if condition is met
if (shape.WidthInch == 3)
{
shape.WidthInch = 1;
Console.WriteLine("Modified shape width (inches): " + shape.WidthInch);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
