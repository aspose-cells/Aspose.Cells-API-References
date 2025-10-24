##Axis.Bins
Axis property. Represents bins on a chartHistogram/Pareto axis
## Axis.Bins property
Represents bins on a chart(Histogram/Pareto) axis
```csharp
public AxisBins Bins { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyBinsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["A4"].PutValue(40);
worksheet.Cells["A5"].PutValue(50);
// Create histogram chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Histogram, 5, 0, 25, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:A5", true);
// Configure bins
AxisBins bins = chart.ValueAxis.Bins;
bins.IsAutomatic = false;
bins.Width = 15;
bins.Overflow = 55;
bins.Underflow = 5;
workbook.Save("AxisBinsDemo.xlsx");
}
}
}
```
### See Also
* class [AxisBins](../../axisbins/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
