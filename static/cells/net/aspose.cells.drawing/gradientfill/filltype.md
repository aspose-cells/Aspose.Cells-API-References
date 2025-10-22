##GradientFill.FillType
GradientFill property. Gets the gradient fill type
## GradientFill.FillType property
Gets the gradient fill type.
```csharp
public GradientFillType FillType { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class GradientFillPropertyFillTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a shape with gradient fill
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
FillFormat fillFormat = shape.Fill;
fillFormat.FillType = FillType.Gradient;
// Set gradient properties
GradientFill gradientFill = fillFormat.GradientFill;
gradientFill.SetTwoColorGradient(System.Drawing.Color.Red, System.Drawing.Color.Blue, GradientStyleType.Horizontal, 1);
// Display the gradient fill type
Console.WriteLine("Gradient Fill Type: " + gradientFill.FillType);
// Change to radial gradient
gradientFill.SetGradient(GradientFillType.Radial, 45, GradientDirectionType.FromCenter);
Console.WriteLine("Updated Gradient Fill Type: " + gradientFill.FillType);
// Save the workbook
workbook.Save("GradientFillDemo.xlsx");
}
}
}
```
### See Also
* enum [GradientFillType](../../gradientfilltype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
