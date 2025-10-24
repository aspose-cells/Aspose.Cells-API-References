##Class AxisBins
Aspose.Cells.Charts.AxisBins class. Represents axis bins
## AxisBins class
Represents axis bins
```csharp
public class AxisBins
```
## Properties
| Name | Description |
| --- | --- |
| [Count](../../aspose.cells.charts/axisbins/count/) { get; set; } | Gets or set the count of axis bins |
| [IsAutomatic](../../aspose.cells.charts/axisbins/isautomatic/) { get; set; } | Indicates whether the axis bins are automatic. |
| [IsByCategory](../../aspose.cells.charts/axisbins/isbycategory/) { get; set; } | Indicates whether grouping data by category |
| [Overflow](../../aspose.cells.charts/axisbins/overflow/) { get; set; } | Gets or set the overflow of axis bins |
| [Underflow](../../aspose.cells.charts/axisbins/underflow/) { get; set; } | Gets or set the underflow of axis bins |
| [Width](../../aspose.cells.charts/axisbins/width/) { get; set; } | Gets or sets the width of axis bin |
## Methods
| Name | Description |
| --- | --- |
| [ResetOverflow](../../aspose.cells.charts/axisbins/resetoverflow/)() | (**Obsolete.**) Reset the overflow |
| [ResetUnderflow](../../aspose.cells.charts/axisbins/resetunderflow/)() | (**Obsolete.**) Reset the underflow |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class AxisBinsDemo
{
public static void AxisBinsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["A4"].PutValue(40);
worksheet.Cells["A5"].PutValue(50);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Histogram, 5, 0, 25, 10);
Chart chart = worksheet.Charts[chartIndex];
// Add data series to the chart
chart.NSeries.Add("A1:A5", true);
// Access the value axis
Axis valueAxis = chart.ValueAxis;
// Access the bins of the value axis
AxisBins bins = valueAxis.Bins;
// Set properties for the bins
bins.IsByCategory = false;
bins.IsAutomatic = true;
bins.Width = 10.0;
bins.Count = 5;
bins.Overflow = 60.0;
bins.Underflow = 0.0;
// Reset overflow and underflow
//bins.ResetOverflow();
//bins.ResetUnderflow();
// Save the workbook
workbook.Save("AxisBinsExample.xlsx");
workbook.Save("AxisBinsExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
