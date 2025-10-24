##Style.GetTwoColorGradientSetting
Style method. Get the twocolor gradient setting
## Style.GetTwoColorGradientSetting method
Get the two-color gradient setting.
```csharp
public TwoColorGradient GetTwoColorGradientSetting()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class StyleMethodGetTwoColorGradientSettingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a style and set two-color gradient
Style style = workbook.CreateStyle();
style.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 1);
style.IsGradient = true;
// Apply the style to a cell
Cell cell = worksheet.Cells["A1"];
cell.PutValue("Two Color Gradient Demo");
cell.SetStyle(style);
try
{
// Call the GetTwoColorGradientSetting method
TwoColorGradient gradientSetting = style.GetTwoColorGradientSetting();
// Display the gradient settings
Console.WriteLine("Color1: " + gradientSetting.Color1);
Console.WriteLine("Color2: " + gradientSetting.Color2);
Console.WriteLine("GradientStyleType: " + gradientSetting.GradientStyleType);
Console.WriteLine("Variant: " + gradientSetting.Variant);
// Modify the gradient settings
gradientSetting.Color1 = Color.Green;
gradientSetting.GradientStyleType = GradientStyleType.Vertical;
style.SetTwoColorGradient(gradientSetting.Color1, gradientSetting.Color2,
gradientSetting.GradientStyleType, gradientSetting.Variant);
Console.WriteLine("Gradient settings modified successfully");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetTwoColorGradientSetting method: {ex.Message}");
}
// Save the result
workbook.Save("MethodGetTwoColorGradientSettingDemo.xlsx");
}
}
}
```
### See Also
* class [TwoColorGradient](../../twocolorgradient/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
