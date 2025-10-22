##FillFormat.SetTwoColorGradient
FillFormat method. Sets the specified fill to a twocolor gradient. Only applies for Excel 2007
## SetTwoColorGradient(Color, Color, GradientStyleType, int) {#settwocolorgradient_1}
Sets the specified fill to a two-color gradient. Only applies for Excel 2007.
```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType style, int variant)
```
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | Color | One gradient color. |
| color2 | Color | Two gradient color. |
| style | GradientStyleType | Gradient shading style. |
| variant | Int32 | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class FillFormatMethodSetTwoColorGradientWithColorColorGradientStyleTypeIntDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a simple shape to demonstrate gradient fill
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 100, 100);
// Get the fill format of the shape
FillFormat fillFormat = shape.Fill;
// Set two-color gradient with specified parameters
fillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.DiagonalDown, 1);
// Save the workbook
workbook.Save("TwoColorGradientDemo.xlsx");
}
}
}
```
### See Also
* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
## SetTwoColorGradient(Color, double, Color, double, GradientStyleType, int) {#settwocolorgradient}
Sets the specified fill to a two-color gradient. Only applies for Excel 2007.
```csharp
public void SetTwoColorGradient(Color color1, double transparency1, Color color2,
double transparency2, GradientStyleType style, int variant)
```
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | Color | One gradient color. |
| transparency1 | Double | The degree of transparency of the color1 as a value from 0.0 (opaque) through 1.0 (clear). |
| color2 | Color | Two gradient color. |
| transparency2 | Double | The degree of transparency of the color2 as a value from 0.0 (opaque) through 1.0 (clear). |
| style | GradientStyleType | Gradient shading style. |
| variant | Int32 | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class FillFormatMethodSetTwoColorGradientWithColorDoubleColorDoubleGradientDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a rectangle shape to demonstrate fill formatting
var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 150, 100);
FillFormat fillFormat = rectangle.Fill;
try
{
// Prepare parameters for SetTwoColorGradient
Color color1 = Color.Red;
double transparency1 = 0.3;
Color color2 = Color.Blue;
double transparency2 = 0.7;
GradientStyleType gradientStyle = GradientStyleType.Horizontal;
int variant = 1;
// Call SetTwoColorGradient with specific parameters
fillFormat.SetTwoColorGradient(
color1,
transparency1,
color2,
transparency2,
gradientStyle,
variant
);
Console.WriteLine("SetTwoColorGradient executed successfully with parameters (Color, Double, Color, Double, GradientStyleType, Int32)");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetTwoColorGradient: {ex.Message}");
}
// Save the workbook to show the effect
workbook.Save("SetTwoColorGradientDemo.xlsx");
}
}
}
```
### See Also
* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
