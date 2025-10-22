##Line.ThemeColor
Line property. Gets and sets the theme color
## Line.ThemeColor property
Gets and sets the theme color.
```csharp
public ThemeColor ThemeColor { get; set; }
```
### Remarks
If the foreground color is not a theme color, NULL will be returned.
### Examples
```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class LinePropertyThemeColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["B1"].PutValue("Series 1");
sheet.Cells["C1"].PutValue("Series 2");
for (int i = 2; i <= 6; i++)
{
sheet.Cells["A" + i].PutValue("Cat " + (i-1));
sheet.Cells["B" + i].PutValue(i * 10);
sheet.Cells["C" + i].PutValue(i * 15);
}
// Add a line chart
int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
Chart chart = sheet.Charts[chartIndex];
// Set chart data range
chart.SetChartDataRange("B1:C6", true);
chart.NSeries.CategoryData = "A2:A6";
// Customize series appearance with ThemeColor
var seriesThemes = new List<ThemeColorType> {
ThemeColorType.Accent1,
ThemeColorType.Accent2
};
for (int i = 0; i < chart.NSeries.Count; i++)
{
chart.NSeries[i].Border.ThemeColor = new ThemeColor(seriesThemes[i], 0.6);
chart.NSeries[i].Border.Style = LineType.Solid;
chart.NSeries[i].Border.Weight = WeightType.MediumLine;
}
// Save the workbook
workbook.Save("LineChartWithThemeColor.xlsx");
}
}
}
```
### See Also
* class [ThemeColor](../../../aspose.cells/themecolor/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
