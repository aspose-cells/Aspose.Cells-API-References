##Legend.Position
Legend property. Gets or sets the legend position type
## Legend.Position property
Gets or sets the legend position type.
```csharp
public LegendPositionType Position { get; set; }
```
### Remarks
Default position is right.If the legend is at left or right side of the chart, setting Legend.X property will not take effect.If the legend is at top or bottom side of the chart, setting Legend.Y property will not take effect.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class LegendPropertyPositionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for chart
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["A2"].PutValue("A");
sheet.Cells["A3"].PutValue("B");
sheet.Cells["A4"].PutValue("C");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["B3"].PutValue(20);
sheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
// Set legend position
chart.Legend.Position = LegendPositionType.Left;
// Save the workbook
workbook.Save("LegendPositionDemo.xlsx");
}
}
}
```
### See Also
* enum [LegendPositionType](../../legendpositiontype/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
