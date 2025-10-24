##GradientFill.GradientStops
GradientFill property. Represents the gradient stop collection
## GradientFill.GradientStops property
Represents the gradient stop collection.
```csharp
public GradientStopCollection GradientStops { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class GradientFillPropertyGradientStopsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ShapeCollection shapes = worksheet.Shapes;
// Add a rectangle shape
Shape shape = shapes.AddRectangle(1, 0, 1, 0, 100, 100);
// Set gradient fill
shape.Fill.FillType = FillType.Gradient;
GradientFill gradientFill = shape.Fill.GradientFill;
// Clear any existing gradient stops
gradientFill.GradientStops.Clear();
// Add custom gradient stops
gradientFill.GradientStops.Add(0.0, Color.Red, 255);
gradientFill.GradientStops.Add(0.5, Color.Yellow, 255);
gradientFill.GradientStops.Add(1.0, Color.Green, 255);
// Demonstrate accessing gradient stops
Console.WriteLine("Gradient Stops Count: " + gradientFill.GradientStops.Count);
Console.WriteLine("First Stop Position: " + gradientFill.GradientStops[0].Position);
Console.WriteLine("Second Stop Color: " + gradientFill.GradientStops[1].CellsColor);
workbook.Save("GradientFillDemo.xlsx");
}
}
}
```
### See Also
* class [GradientStopCollection](../../gradientstopcollection/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
