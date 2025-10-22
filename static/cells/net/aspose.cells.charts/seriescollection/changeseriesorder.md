##SeriesCollection.ChangeSeriesOrder
SeriesCollection method. Directly changes the orders of the two series
## SeriesCollection.ChangeSeriesOrder method
Directly changes the orders of the two series.
```csharp
[Obsolete("Use SeriesCollection.SwapSeries property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ChangeSeriesOrder(int sourceIndex, int destIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | Int32 | The current index |
| destIndex | Int32 | The dest index |
### Remarks
NOTE: This method is now obsolete. Instead, please use SeriesCollection.SwapSeries method. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class SeriesCollectionMethodChangeSeriesOrderWithInt32Int32Demo
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
worksheet.Cells["B2"].PutValue(40);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["B4"].PutValue(60);
worksheet.Cells["C1"].PutValue("Series 3");
worksheet.Cells["C2"].PutValue(70);
worksheet.Cells["C3"].PutValue(80);
worksheet.Cells["C4"].PutValue(90);
// Create a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add series to the chart
chart.NSeries.Add("A2:A4", true);
chart.NSeries.Add("B2:B4", true);
chart.NSeries.Add("C2:C4", true);
// Get the series collection
SeriesCollection seriesCollection = chart.NSeries;
try
{
// Call the ChangeSeriesOrder method to swap series at index 0 and 2
seriesCollection.ChangeSeriesOrder(0, 2);
Console.WriteLine("Series order changed successfully. Series at index 0 and 2 swapped.");
// Display the new series order
for (int i = 0; i < seriesCollection.Count; i++)
{
Console.WriteLine($"Series {i + 1}: {seriesCollection[i].Name}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ChangeSeriesOrder method: {ex.Message}");
}
// Save the result
workbook.Save("ChangeSeriesOrderWithInt32Int32Demo.xlsx");
}
}
}
```
### See Also
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
