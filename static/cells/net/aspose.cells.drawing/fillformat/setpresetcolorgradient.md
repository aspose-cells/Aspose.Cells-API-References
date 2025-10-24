##FillFormat.SetPresetColorGradient
FillFormat method. Sets the specified fill to a presetcolor gradient. Only applies for Excel 2007
## FillFormat.SetPresetColorGradient method
Sets the specified fill to a preset-color gradient. Only applies for Excel 2007.
```csharp
public void SetPresetColorGradient(GradientPresetType presetColor, GradientStyleType style,
int variant)
```
| Parameter | Type | Description |
| --- | --- | --- |
| presetColor | GradientPresetType | Preset color type |
| style | GradientStyleType | Gradient shading style. |
| variant | Int32 | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class FillFormatMethodSetPresetColorGradientWithGradientPresetTypeGradientStylDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["B1"].PutValue("Value");
for (int i = 2; i <= 5; i++)
{
sheet.Cells[$"A{i}"].PutValue($"Item {i-1}");
sheet.Cells[$"B{i}"].PutValue(i * 10);
}
// Create chart
int chartIndex = sheet.Charts.Add(ChartType.Column, 8, 0, 20, 10);
Chart chart = sheet.Charts[chartIndex];
chart.NSeries.Add("B2:B5", true);
chart.NSeries.CategoryData = "A2:A5";
// Apply gradient fill
FillFormat fillFormat = chart.PlotArea.Area.FillFormat;
fillFormat.SetPresetColorGradient(GradientPresetType.Daybreak, GradientStyleType.Vertical, 1);
// Save the workbook
workbook.Save("SetPresetColorGradientDemo.xlsx");
}
}
}
```
### See Also
* enum [GradientPresetType](../../gradientpresettype/)
* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
