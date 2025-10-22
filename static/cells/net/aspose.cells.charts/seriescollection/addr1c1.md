##SeriesCollection.AddR1C1
SeriesCollection method. Adds the Series collection to a chart
## SeriesCollection.AddR1C1 method
Adds the [`Series`](../../series/) collection to a chart.
```csharp
public int AddR1C1(string area, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| area | String | Specifies values from which to plot the data series |
| isVertical | Boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
### Return Value
Return the first index of the added ASeries in the NSeries.
### Remarks
If set data on contiguous cells, use colon to seperate them.For example, R[1]C[1]:R[3]C[2].If set data on contiguous cells, use comma to seperate them.For example,(R[1]C[1],R[3]C[2]).
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesCollectionMethodAddR1C1WithStringBooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet wsData = workbook.Worksheets[0];
wsData.Name = "ChartData";
// Sample data
wsData.Cells[0, 0].PutValue(1);
wsData.Cells[1, 0].PutValue(2);
wsData.Cells[0, 1].PutValue(3);
wsData.Cells[1, 1].PutValue(4);
Worksheet wsChart = workbook.Worksheets[workbook.Worksheets.Add(Aspose.Cells.SheetType.Chart)];
wsChart.Name = "ChartSheet";
int chartIndex = wsChart.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 0, 0, 15, 15);
Aspose.Cells.Charts.Chart chart = wsChart.Charts[chartIndex];
// Using AddR1C1 with String and Boolean parameters
int seriesIndex = chart.NSeries.AddR1C1("ChartData!R1C2:R2C2", true);
Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];
series.XValues = "ChartData!R1C1:R2C1";
workbook.Save("SeriesCollectionAddR1C1Demo.xlsx", Aspose.Cells.SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
