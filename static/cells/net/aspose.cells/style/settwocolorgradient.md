##Style.SetTwoColorGradient
Style method. Sets the specified fill to a twocolor gradient
## Style.SetTwoColorGradient method
Sets the specified fill to a two-color gradient.
```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType gradientStyleType,
int variant)
```
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | Color | One gradient color. |
| color2 | Color | Two gradient color. |
| gradientStyleType | GradientStyleType | Gradient shading style. |
| variant | Int32 | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class StyleMethodSetTwoColorGradientWithColorColorGradientStyleTypeIntDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a style object
Style style = workbook.CreateStyle();
// Set two color gradient for the style
style.SetTwoColorGradient(Color.Green, Color.Red, GradientStyleType.Vertical, 1);
// Apply the style to a cell
Cell cell = worksheet.Cells["A1"];
cell.SetStyle(style);
cell.PutValue("Gradient Style Demo");
// Verify the gradient settings
Color color1, color2;
GradientStyleType gradientStyle;
int variant;
style.GetTwoColorGradient(out color1, out color2, out gradientStyle, out variant);
Console.WriteLine("Color1: " + color1);
Console.WriteLine("Color2: " + color2);
Console.WriteLine("Gradient Style: " + gradientStyle);
Console.WriteLine("Variant: " + variant);
// Save the workbook
workbook.Save("TwoColorGradientDemo.xlsx");
}
}
}
```
### See Also
* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
