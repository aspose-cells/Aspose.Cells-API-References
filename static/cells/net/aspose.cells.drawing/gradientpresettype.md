##Enum GradientPresetType
Aspose.Cells.Drawing.GradientPresetType enum. Represents gradient preset color type
## GradientPresetType enumeration
Represents gradient preset color type.
```csharp
public enum GradientPresetType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Brass | `0` | Brass preset color |
| CalmWater | `1` | Calm Water preset color |
| Chrome | `2` | Chrome preset color |
| ChromeII | `3` | Chrome II preset color |
| Daybreak | `4` | Daybreak preset color |
| Desert | `5` | Desert preset color |
| EarlySunset | `6` | Early Sunset preset color |
| Fire | `7` | Fire preset color |
| Fog | `8` | Fog preset color |
| Gold | `9` | Gold preset color |
| GoldII | `10` | Gold II preset color |
| Horizon | `11` | Horizon preset color |
| LateSunset | `12` | Late Sunset preset color |
| Mahogany | `13` | Mahogany preset color |
| Moss | `14` | Moss preset color |
| Nightfall | `15` | Nightfall preset color |
| Ocean | `16` | Ocean preset color |
| Parchment | `17` | Parchment preset color |
| Peacock | `18` | Peacock preset color |
| Rainbow | `19` | Rainbow preset color |
| RainbowII | `20` | Rainbow II preset color |
| Sapphire | `21` | Sapphire preset color |
| Silver | `22` | Silver preset color |
| Wheat | `23` | Wheat preset color |
| Unknown | `24` | Unknown preset color. Only for the preset color (which is not same as any known preset color) in the template workbook. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class GradientPresetTypeDemo
{
public static void GradientPresetTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set the chart data range
chart.SetChartDataRange("A1:B4", true);
// Access the chart's category axis
Axis categoryAxis = chart.CategoryAxis;
// Access the fill format of the category axis area
FillFormat fillFormat = categoryAxis.Area.FillFormat;
// Set a gradient preset color for the fill format
fillFormat.SetPresetColorGradient(GradientPresetType.Fire, GradientStyleType.Horizontal, 1);
// Output the gradient preset color type
Console.WriteLine("Gradient Preset Color: " + fillFormat.PresetColor);
// Save the workbook
workbook.Save("GradientPresetTypeExample.xlsx");
workbook.Save("GradientPresetTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
