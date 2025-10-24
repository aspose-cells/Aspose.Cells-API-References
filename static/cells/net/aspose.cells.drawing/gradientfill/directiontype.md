##GradientFill.DirectionType
GradientFill property. Gets the gradient direction type
## GradientFill.DirectionType property
Gets the gradient direction type.
```csharp
public GradientDirectionType DirectionType { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class GradientFillPropertyDirectionTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a shape to demonstrate gradient fill
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 5, 5);
// Set gradient fill properties
FillFormat fillFormat = shape.Fill;
fillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.LightBlue, GradientStyleType.DiagonalDown, 1);
fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);
// Output the gradient direction type
Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);
// Save the workbook
workbook.Save("GradientDirectionTypeExample.xlsx");
}
}
}
```
### See Also
* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
