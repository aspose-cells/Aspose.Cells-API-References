##GradientFill.SetPresetThemeGradient
GradientFill method. Sets preset theme gradient fill
## GradientFill.SetPresetThemeGradient method
Sets preset theme gradient fill.
```csharp
public void SetPresetThemeGradient(PresetThemeGradientType gradientType,
ThemeColorType themeColorType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| gradientType | PresetThemeGradientType | The preset gradient type. |
| themeColorType | ThemeColorType | The theme color type. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class GradientFillMethodSetPresetThemeGradientWithPresetThemeGradientTypeThemeCoDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Sample");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(20);
worksheet.Cells["A4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.SetChartDataRange("A1:A4", false);
// Configure series fill with gradient
Aspose.Cells.Charts.Series series = chart.NSeries[0];
series.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Gradient;
// Demonstrate SetPresetThemeGradient with specified parameters
series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
Aspose.Cells.Drawing.PresetThemeGradientType.RadialGradient,
Aspose.Cells.ThemeColorType.Accent1);
// Save the workbook
workbook.Save("GradientFillDemo.xlsx");
}
}
}
```
### See Also
* enum [PresetThemeGradientType](../../presetthemegradienttype/)
* enum [ThemeColorType](../../../aspose.cells/themecolortype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
