##SeriesLayoutProperties.IsIntervalLeftClosed
SeriesLayoutProperties property. Indicates whether the interval is closed on the left side
## SeriesLayoutProperties.IsIntervalLeftClosed property
Indicates whether the interval is closed on the left side.
```csharp
public bool IsIntervalLeftClosed { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesLayoutPropertiesPropertyIsIntervalLeftClosedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["B1"].PutValue(15);
worksheet.Cells["B2"].PutValue(25);
worksheet.Cells["B3"].PutValue(35);
// Create chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
int seriesIndex = chart.NSeries.Add("A1:B3", true);
Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];
// Set IsIntervalLeftClosed property
series.LayoutProperties.IsIntervalLeftClosed = true;
// Save workbook
workbook.Save("SeriesLayoutPropertiesIsIntervalLeftClosedDemo.xlsx");
}
}
}
```
### See Also
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
