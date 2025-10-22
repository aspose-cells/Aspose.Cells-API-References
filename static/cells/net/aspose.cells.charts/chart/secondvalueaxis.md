##Chart.SecondValueAxis
Chart property. Gets the charts second Y axis
## Chart.SecondValueAxis property
Gets the chart's second Y axis.
```csharp
public Axis SecondValueAxis { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertySecondValueAxisDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Series 1");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(300);
worksheet.Cells["C1"].PutValue("Series 2");
worksheet.Cells["C2"].PutValue(5000);
worksheet.Cells["C3"].PutValue(3000);
worksheet.Cells["C4"].PutValue(1000);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.Add("C2:C4", true);
chart.NSeries.CategoryData = "A2:A4";
// Enable secondary value axis for the second series
chart.NSeries[1].PlotOnSecondAxis = true;
// Customize the secondary value axis
Axis secondValueAxis = chart.SecondValueAxis;
secondValueAxis.Title.Text = "Secondary Axis";
secondValueAxis.MinValue = 0;
secondValueAxis.MaxValue = 6000;
secondValueAxis.MajorUnit = 1000;
// Save the workbook
workbook.Save("SecondValueAxisDemo.xlsx");
}
}
}
```
### See Also
* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
