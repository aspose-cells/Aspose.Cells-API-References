##TrendlineCollection.Item
TrendlineCollection property. Gets a Trendline object by its index
## TrendlineCollection indexer
Gets a [`Trendline`](../../trendline/) object by its index.
```csharp
public Trendline this[int index] { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TrendlineCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue(1);
sheet.Cells["A2"].PutValue(2);
sheet.Cells["A3"].PutValue(3);
sheet.Cells["B1"].PutValue(4);
sheet.Cells["B2"].PutValue(5);
sheet.Cells["B3"].PutValue(6);
// Add a chart
int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
Chart chart = sheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("A1:A3", true);
chart.NSeries[0].Values = "B1:B3";
// Add a trendline
int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
// Demonstrate Item property usage
Trendline firstTrendline = chart.NSeries[0].TrendLines[0];
Console.WriteLine("Trendline Type: " + firstTrendline.Type);
}
}
}
```
### See Also
* class [Trendline](../../trendline/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
