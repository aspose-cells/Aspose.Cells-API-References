##GradientFill.Angle
GradientFill property. The angle of linear fill
## GradientFill.Angle property
The angle of linear fill.
```csharp
public float Angle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class GradientFillPropertyAngleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate gradient fill
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);
// Set gradient fill properties
shape.Fill.FillType = FillType.Gradient;
shape.Fill.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromCenter);
shape.Fill.GradientFill.Angle = 45; // Set the angle to 45 degrees
// Set gradient colors
shape.Fill.GradientFill.SetTwoColorGradient(
Color.Red,
Color.Blue,
GradientStyleType.Horizontal,
1);
// Save the workbook
workbook.Save("GradientFillAngleDemo.xlsx");
Console.WriteLine("Demo completed. File saved with gradient fill at 45 degree angle.");
}
}
}
```
### See Also
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
