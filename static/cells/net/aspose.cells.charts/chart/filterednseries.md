##Chart.FilteredNSeries
Chart property. Gets a SeriesCollection collection representing the data series that are filtered in the chart
## Chart.FilteredNSeries property
Gets a [`SeriesCollection`](../../seriescollection/) collection representing the data series that are filtered in the chart.
```csharp
public SeriesCollection FilteredNSeries { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyFilteredNSeriesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Series");
worksheet.Cells["A2"].PutValue("Series 1");
worksheet.Cells["A3"].PutValue("Series 2");
worksheet.Cells["A4"].PutValue("Series 3");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart and set some series as filtered
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Filter some series (hide Series 2)
chart.NSeries[1].IsFiltered = true;
// Access filtered series collection
Aspose.Cells.Charts.SeriesCollection filteredSeries = chart.FilteredNSeries;
Console.WriteLine("Filtered Series Count: " + filteredSeries.Count.ToString());
// Save the workbook
workbook.Save("FilteredNSeriesDemo.xlsx");
}
}
}
```
### See Also
* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
