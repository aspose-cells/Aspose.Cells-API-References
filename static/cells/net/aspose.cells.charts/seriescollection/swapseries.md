##SeriesCollection.SwapSeries
SeriesCollection method. Directly changes the orders of the two series
## SeriesCollection.SwapSeries method
Directly changes the orders of the two series.
```csharp
public void SwapSeries(int sourceIndex, int destIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | Int32 | The current index |
| destIndex | Int32 | The dest index |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesCollectionMethodSwapSeriesWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Series 1");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(20);
worksheet.Cells["A4"].PutValue(30);
worksheet.Cells["B1"].PutValue("Series 2");
worksheet.Cells["B2"].PutValue(5);
worksheet.Cells["B3"].PutValue(10);
worksheet.Cells["B4"].PutValue(15);
worksheet.Cells["C1"].PutValue("Series 3");
worksheet.Cells["C2"].PutValue(8);
worksheet.Cells["C3"].PutValue(16);
worksheet.Cells["C4"].PutValue(24);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("A1:C4", true);
// Get the series collection
Aspose.Cells.Charts.SeriesCollection sc = chart.NSeries;
// Print original series names
Console.WriteLine("Original Series Order:");
for (int i = 0; i < sc.Count; i++)
{
Console.WriteLine($"Series {i}: {sc[i].Name}");
}
// Swap series 0 and 1
sc.SwapSeries(0, 1);
Console.WriteLine("\nAfter swapping series 0 and 1:");
for (int i = 0; i < sc.Count; i++)
{
Console.WriteLine($"Series {i}: {sc[i].Name}");
}
// Swap series 2 and 0
sc.SwapSeries(2, 0);
Console.WriteLine("\nAfter swapping series 2 and 0:");
for (int i = 0; i < sc.Count; i++)
{
Console.WriteLine($"Series {i}: {sc[i].Name}");
}
}
}
}
```
### See Also
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
