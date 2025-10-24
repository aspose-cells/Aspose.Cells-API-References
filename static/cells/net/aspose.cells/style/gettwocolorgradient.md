##Style.GetTwoColorGradient
Style method. Get the twocolor gradient setting
## Style.GetTwoColorGradient method
Get the two-color gradient setting.
```csharp
[Obsolete("Use Style.GetTwoColorGradientSetting() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GetTwoColorGradient(out Color color1, out Color color2,
out GradientStyleType gradientStyleType, out int variant)
```
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | Color& | One gradient color. |
| color2 | Color& | Two gradient color. |
| gradientStyleType | GradientStyleType& | Gradient shading style. |
| variant | Int32& | The gradient variant. |
### Remarks
NOTE: This method is now obsolete. Instead, please use Style.GetTwoColorGradientSetting() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class StyleMethodGetTwoColorGradientWithColorColorGradientStyleTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a style and set two color gradient
Style style = workbook.CreateStyle();
style.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 1);
// Apply the style to a cell
Cell cell = worksheet.Cells["A1"];
cell.SetStyle(style);
cell.PutValue("Two Color Gradient Demo");
// Prepare variables to get gradient settings
Color color1 = Color.Empty;
Color color2 = Color.Empty;
GradientStyleType gradientStyle = GradientStyleType.Horizontal;
int variant = 0;
try
{
// Call the GetTwoColorGradient method
#pragma warning disable CS0618 // Type or member is obsolete
style.GetTwoColorGradient(out color1, out color2, out gradientStyle, out variant);
#pragma warning restore CS0618 // Type or member is obsolete
// Display the retrieved gradient settings
Console.WriteLine("Gradient Settings:");
Console.WriteLine($"Color1: {color1}");
Console.WriteLine($"Color2: {color2}");
Console.WriteLine($"Gradient Style: {gradientStyle}");
Console.WriteLine($"Variant: {variant}");
// Save the workbook
workbook.Save("StyleMethodGetTwoColorGradientDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetTwoColorGradient method: {ex.Message}");
}
}
}
}
```
### See Also
* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
