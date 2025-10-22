##Shape.HeightInch
Shape property. Represents the height of the shape in unit of inches
## Shape.HeightInch property
Represents the height of the shape, in unit of inches.
```csharp
public double HeightInch { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ShapePropertyHeightInchDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);
// Set and get height in inches
shape.HeightInch = 3;
Console.WriteLine("Shape height (inches): " + shape.HeightInch);
// Modify height if condition is met
if (shape.HeightInch == 3)
{
shape.HeightInch = 1;
Console.WriteLine("Modified shape height (inches): " + shape.HeightInch);
}
}
}
}
```
### See Also
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
