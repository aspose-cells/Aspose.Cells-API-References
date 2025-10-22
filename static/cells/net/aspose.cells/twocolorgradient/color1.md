##TwoColorGradient.Color1
TwoColorGradient property. Gets and sets the first gradient color
## TwoColorGradient.Color1 property
Gets and sets the first gradient color.
```csharp
public Color Color1 { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
public class TwoColorGradientPropertyColor1Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["A1"];
// Create style with gradient fill
Style style = workbook.CreateStyle();
style.Pattern = BackgroundType.Solid;
// Initialize two-color gradient
style.SetTwoColorGradient(
Color.Red,
Color.Blue,
GradientStyleType.Vertical,
variant: 1);
// Apply gradient to cell style
cell.SetStyle(style);
// Read initial color
TwoColorGradient gradient = style.GetTwoColorGradientSetting();
Console.WriteLine("Current Color1 value: " + gradient.Color1);
// Modify gradient color and reapply
gradient.Color1 = Color.Lime;
style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
// Verify update
Console.WriteLine("Updated Color1 value: " + gradient.Color1);
// Visual demonstration in output file
cell.PutValue("Color1 Gradient Demo");
worksheet.AutoFitColumn(0);
workbook.Save("TwoColorGradientPropertyColor1Demo.xlsx");
}
}
}
```
### See Also
* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
