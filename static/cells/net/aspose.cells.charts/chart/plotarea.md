##Chart.PlotArea
Chart property. Gets the charts plot area which includes axis tick labels
## Chart.PlotArea property
Gets the chart's plot area which includes axis tick labels.
```csharp
public PlotArea PlotArea { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ChartPropertyPlotAreaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
// Customize plot area
chart.PlotArea.Area.FillFormat.FillType = FillType.Solid;
chart.PlotArea.Area.FillFormat.SolidFill.Color = Color.LightBlue;
chart.PlotArea.Border.Color = Color.Black;
// Save the workbook
workbook.Save("ChartPlotAreaDemo.xlsx");
}
}
}
```
### See Also
* class [PlotArea](../../plotarea/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
