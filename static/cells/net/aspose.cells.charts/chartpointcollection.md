##Class ChartPointCollection
Aspose.Cells.Charts.ChartPointCollection class. Represents a collection that contains all the points in one series
## ChartPointCollection class
Represents a collection that contains all the points in one series.
```csharp
public class ChartPointCollection : IEnumerable
```
## Properties
| Name | Description |
| --- | --- |
| [Count](../../aspose.cells.charts/chartpointcollection/count/) { get; } | Gets the count of the chart point. |
| [Item](../../aspose.cells.charts/chartpointcollection/item/) { get; } | Gets the [`ChartPoint`](../chartpoint/) element at the specified index in the series. |
## Methods
| Name | Description |
| --- | --- |
| [Clear](../../aspose.cells.charts/chartpointcollection/clear/)() | Remove all setting of the chart points. |
| [GetEnumerator](../../aspose.cells.charts/chartpointcollection/getenumerator/)() | Returns an enumerator for the entire `ChartPointCollection`. |
| [RemoveAt](../../aspose.cells.charts/chartpointcollection/removeat/)(int) | Removes point at the index of the series.. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartPointCollectionDemo
{
public static void ChartPointCollectionExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Adding sample values to cells
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
// Adding a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.PieExploded, 5, 0, 25, 10);
// Accessing the instance of the newly added chart
Chart chart = worksheet.Charts[chartIndex];
// Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", true);
// Show Data Labels
chart.NSeries[0].DataLabels.ShowValue = true;
// Accessing the ChartPointCollection
ChartPointCollection points = chart.NSeries[0].Points;
// Iterating through the points in the collection
for (int i = 0; i < points.Count; i++)
{
// Get Data Point
ChartPoint point = points[i];
// Set Pie Explosion
point.Explosion = 15;
// Set Border Color
point.Border.Color = System.Drawing.Color.Red;
}
// Saving the Excel file
workbook.Save("ChartPointCollectionExample.xlsx");
workbook.Save("ChartPointCollectionExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
