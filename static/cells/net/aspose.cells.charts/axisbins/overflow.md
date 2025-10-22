##AxisBins.Overflow
AxisBins property. Gets or set the overflow of axis bins
## AxisBins.Overflow property
Gets or set the overflow of axis bins
```csharp
public double Overflow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisBinsPropertyOverflowDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["A4"].PutValue(40);
worksheet.Cells["A5"].PutValue(50);
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Histogram, 5, 0, 25, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:A5", true);
Axis valueAxis = chart.ValueAxis;
AxisBins bins = valueAxis.Bins;
bins.IsAutomatic = false;
bins.Width = 10;
bins.Overflow = 60.0;
workbook.Save("AxisBinsOverflowDemo.xlsx");
}
}
}
```
### See Also
* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
