##Class GradientFill
Aspose.Cells.Drawing.GradientFill class. Represents the gradient fill
## GradientFill class
Represents the gradient fill.
```csharp
public class GradientFill : Fill
```
## Properties
| Name | Description |
| --- | --- |
| [Angle](../../aspose.cells.drawing/gradientfill/angle/) { get; set; } | The angle of linear fill. |
| [DirectionType](../../aspose.cells.drawing/gradientfill/directiontype/) { get; } | Gets the gradient direction type. |
| [FillType](../../aspose.cells.drawing/gradientfill/filltype/) { get; } | Gets the gradient fill type. |
| [GradientStops](../../aspose.cells.drawing/gradientfill/gradientstops/) { get; } | Represents the gradient stop collection. |
## Methods
| Name | Description |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Inherited from [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Gets the hash code.(Inherited from [`Fill`](../fill/).) |
| [SetGradient](../../aspose.cells.drawing/gradientfill/setgradient/)(GradientFillType, double, GradientDirectionType) | Set the gradient fill type and direction. |
| [SetOneColorGradient](../../aspose.cells.drawing/gradientfill/setonecolorgradient/)(Color, double, GradientStyleType, int) | Sets the specified fill to a one-color gradient. Only applies for Excel 2007. |
| [SetPresetThemeGradient](../../aspose.cells.drawing/gradientfill/setpresetthemegradient/)(PresetThemeGradientType, ThemeColorType) | Sets preset theme gradient fill. |
| [SetTwoColorGradient](../../aspose.cells.drawing/gradientfill/settwocolorgradient/#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/gradientfill/settwocolorgradient/#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
public class DrawingClassGradientFillDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape to the worksheet with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 150, 100);
// Set fill type to gradient to access gradient fill properties
shape.Fill.FillType = FillType.Gradient;
// Get the existing gradient fill instance from the shape
GradientFill gradientFill = shape.Fill.GradientFill;
// Configure the gradient with two colors using the existing instance
gradientFill.SetTwoColorGradient(
Color.LightSkyBlue,  // First color
Color.DarkBlue,      // Second color
GradientStyleType.Horizontal, // Gradient style
1                    // Variant
);
// Save the workbook
workbook.Save("GradientFillDemo.xlsx");
}
}
}
```
### See Also
* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
