##Chart.PlotBy
Chart property. Gets and sets whether plot by row or column
## Chart.PlotBy property
Gets and sets whether plot by row or column.
```csharp
public PlotDataByType PlotBy { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyPlotByDemo
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
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["C1"].PutValue("Series 2");
worksheet.Cells["C2"].PutValue(15);
worksheet.Cells["C3"].PutValue(25);
worksheet.Cells["C4"].PutValue(35);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.SetChartDataRange("A1:C4", true);
// Demonstrate PlotBy property
Console.WriteLine("Default PlotBy: " + chart.PlotBy);
// Create new chart with different plot by setting
int newChartIndex = worksheet.Charts.Add(ChartType.Column, 25, 0, 40, 8);
Aspose.Cells.Charts.Chart newChart = worksheet.Charts[newChartIndex];
newChart.SetChartDataRange("A1:C4", false); // Plot by row
Console.WriteLine("New chart PlotBy: " + newChart.PlotBy);
// Save the workbook
workbook.Save("ChartPropertyPlotByDemo_out.xlsx");
}
}
}
```
### See Also
* enum [PlotDataByType](../../plotdatabytype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
