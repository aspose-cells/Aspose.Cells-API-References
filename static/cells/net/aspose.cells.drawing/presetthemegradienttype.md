##Enum PresetThemeGradientType
Aspose.Cells.Drawing.PresetThemeGradientType enum. Represents the preset theme gradient type
## PresetThemeGradientType enumeration
Represents the preset theme gradient type.
```csharp
public enum PresetThemeGradientType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| LightGradient | `0` | Light gradient |
| TopSpotlight | `1` | Top spotlight |
| MediumGradient | `2` | Medium gradient |
| BottomSpotlight | `3` | Bottom spotlight |
| RadialGradient | `4` | Radial gradient |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class DrawingClassPresetThemeGradientTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Category 1");
worksheet.Cells["A3"].PutValue("Category 2");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
// Add a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B3", true);
// Apply gradient fill to the first series
Aspose.Cells.Charts.Series series = chart.NSeries[0];
series.Area.FillFormat.FillType = FillType.Gradient;
series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
PresetThemeGradientType.RadialGradient,
ThemeColorType.Accent1);
// Save the workbook
workbook.Save("PresetThemeGradientDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
