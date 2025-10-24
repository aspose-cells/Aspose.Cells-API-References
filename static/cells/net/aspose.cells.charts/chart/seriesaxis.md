##Chart.SeriesAxis
Chart property. Gets the charts series axis
## Chart.SeriesAxis property
Gets the chart's series axis.
```csharp
public Axis SeriesAxis { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertySeriesAxisDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Series");
worksheet.Cells["A2"].PutValue("Q1");
worksheet.Cells["A3"].PutValue("Q2");
worksheet.Cells["A4"].PutValue("Q3");
worksheet.Cells["B1"].PutValue("Product A");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(300);
worksheet.Cells["C1"].PutValue("Product B");
worksheet.Cells["C2"].PutValue(150);
worksheet.Cells["C3"].PutValue(250);
worksheet.Cells["C4"].PutValue(350);
// Add a 3D clustered column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B1:C4", true);
// Access and configure the SeriesAxis
Axis seriesAxis = chart.SeriesAxis;
seriesAxis.Title.Text = "Product Series";
seriesAxis.Title.Font.Size = 12;
seriesAxis.Title.Font.IsBold = true;
seriesAxis.MajorTickMark = TickMarkType.Cross;
seriesAxis.MinorTickMark = TickMarkType.Outside;
// Save the workbook
workbook.Save("ChartPropertySeriesAxisDemo.xlsx");
}
}
}
```
### See Also
* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
