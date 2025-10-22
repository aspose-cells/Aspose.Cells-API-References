##GradientFill.SetGradient
GradientFill method. Set the gradient fill type and direction
## GradientFill.SetGradient method
Set the gradient fill type and direction.
```csharp
public void SetGradient(GradientFillType type, double angle, GradientDirectionType direction)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | GradientFillType | Gradient fill type. |
| angle | Double | The angle. Only applies for GradientFillType.Linear. |
| direction | GradientDirectionType | The direction type. Only applies for GradientFillType.Radial and GradientFillType.Rectangle. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class GradientFillMethodSetGradientWithGradientFillTypeDoubleGradientDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to apply gradient fill
Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 100);
try
{
// Get the shape's fill gradient
GradientFill gradientFill = shape.Fill.GradientFill; // Fixed property name from Gradient to GradientFill
if (gradientFill == null)
{
Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
return;
}
// Call SetGradient with specific parameters: Linear fill, 90 degrees, FromCenter direction
gradientFill.SetGradient(GradientFillType.Linear, 90.0, GradientDirectionType.FromCenter);
Console.WriteLine("SetGradient method executed successfully with parameters (GradientFillType.Linear, 90.0, GradientDirectionType.FromCenter)");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetGradient method: {ex.Message}");
}
// Save the workbook to demonstrate the effect
workbook.Save("GradientFillSetGradientDemo.xlsx");
}
}
}
```
### See Also
* enum [GradientFillType](../../gradientfilltype/)
* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
