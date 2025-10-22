##GradientStop.Position
GradientStop property. The position of the stop
## GradientStop.Position property
The position of the stop.
```csharp
public double Position { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class GradientStopPropertyPositionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["A2"].PutValue("A");
sheet.Cells["A3"].PutValue("B");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["B3"].PutValue(20);
// Add a chart
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B3", true);
// Configure gradient fill for the first series
Aspose.Cells.Charts.Series series = chart.NSeries[0];
series.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Gradient;
series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
Aspose.Cells.Drawing.PresetThemeGradientType.RadialGradient,
ThemeColorType.Accent1);
// Access and modify gradient stop positions
GradientStopCollection stops = series.Area.FillFormat.GradientFill.GradientStops;
stops[0].Position = 0;
stops[1].Position = 50;
stops[2].Position = 100;
// Save the workbook
workbook.Save("GradientStopPositionDemo.xlsx");
}
}
}
```
### See Also
* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
