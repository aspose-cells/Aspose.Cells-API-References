##GradientStop.Transparency
GradientStop property. Returns or sets the degree of transparency of the area as a value from 0.0 opaque through 1.0 clear
## GradientStop.Transparency property
Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).
```csharp
public double Transparency { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class GradientStopPropertyTransparencyDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape with gradient fill
Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 300);
shape.Fill.FillType = FillType.Gradient;
GradientFill gradientFill = shape.Fill.GradientFill;
gradientFill.SetGradient(GradientFillType.Linear, 0, GradientDirectionType.FromUpperLeftCorner);
// Create color for gradient stop
CellsColor color = workbook.CreateCellsColor();
color.Color = Color.Blue;
// Add gradient stop with initial transparency
gradientFill.GradientStops.Add(0, color, 30);
// Access the gradient stop
GradientStop stop = gradientFill.GradientStops[0];
// Display and modify transparency
Console.WriteLine("Initial Transparency: " + stop.Transparency);
stop.Transparency = 0.7;
Console.WriteLine("Modified Transparency: " + stop.Transparency);
// Add another stop for visual comparison
CellsColor color2 = workbook.CreateCellsColor();
color2.Color = Color.Green;
gradientFill.GradientStops.Add(1, color2, 30);
// Save the workbook
workbook.Save("GradientStopTransparencyDemo.xlsx");
}
}
}
```
### See Also
* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
