##Chart.NSeries
Chart property. Gets a SeriesCollection collection representing the data series in the chart
## Chart.NSeries property
Gets a [`SeriesCollection`](../../seriescollection/) collection representing the data series in the chart.
```csharp
public SeriesCollection NSeries { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyNSeriesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data to cells
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["B1"].PutValue("Value");
for (int i = 2; i <= 10; i++)
{
sheet.Cells["A" + i].PutValue("Cat " + (i - 1));
sheet.Cells["B" + i].PutValue(i * 10);
}
// Add a chart
int chartIndex = sheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 2, 25, 11);
Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
// Set the data source for the chart series using NSeries
chart.NSeries.Add("=Sheet1!$A$2:$B$10", true);
// Set chart title
chart.Title.Text = "NSeries Demo Chart";
// Save the workbook
workbook.Save("NSeriesDemo.xlsx");
}
}
}
```
### See Also
* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
