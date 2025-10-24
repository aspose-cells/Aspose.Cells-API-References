##SeriesCollection.Item
SeriesCollection property. Gets the Series element at the specified index
## SeriesCollection indexer
Gets the [`Series`](../../series/) element at the specified index.
```csharp
public Series this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class SeriesCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Series");
sheet.Cells["A2"].PutValue(1);
sheet.Cells["A3"].PutValue(2);
sheet.Cells["A4"].PutValue(3);
sheet.Cells["B1"].PutValue("Values");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["B3"].PutValue(20);
sheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = sheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access the first series and its first point using Item property
Series series = chart.NSeries[0];
ChartPoint point = series.Points[0];
// Customize the point appearance
point.Area.FillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.White, GradientStyleType.Vertical, 2);
point.Area.FillFormat.FillType = FillType.Solid;
// Save the workbook
workbook.Save("SeriesCollectionPropertyItemDemo_out.xlsx");
}
}
}
```
### See Also
* class [Series](../../series/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
