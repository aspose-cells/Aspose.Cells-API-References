##ChartPointCollection.Item
ChartPointCollection property. Gets the ChartPoint element at the specified index in the series
## ChartPointCollection indexer
Gets the [`ChartPoint`](../../chartpoint/) element at the specified index in the series.
```csharp
public ChartPoint this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index of chart point in the series. |
### Return Value
The ChartPoint object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ChartPointCollectionPropertyItemDemo
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
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access a specific chart point using Item property
ChartPoint point = chart.NSeries[0].Points[1];
// Modify the point's fill pattern
point.Area.FillFormat.Pattern = FillPattern.LightHorizontal;
// Save the workbook
workbook.Save("ChartPointCollectionPropertyItemDemo.xlsx");
}
}
}
```
### See Also
* class [ChartPoint](../../chartpoint/)
* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
