##Series.XErrorBar
Series property. Represents X direction error bar of the series
## Series.XErrorBar property
Represents X direction error bar of the series.
```csharp
public ErrorBar XErrorBar { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyXErrorBarDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("X Values");
worksheet.Cells["B1"].PutValue("Y Values");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["A4"].PutValue(3);
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Add series using the data
SeriesCollection seriesCollection = chart.NSeries;
seriesCollection.Add("B2:B4", true);
Series series = seriesCollection[0];
series.XValues = "A2:A4";
// Configure XErrorBar properties
series.XErrorBar.DisplayType = ErrorBarDisplayType.Plus;
series.XErrorBar.Amount = 0.5;
series.XErrorBar.Type = ErrorBarType.FixedValue;
// Save the workbook
workbook.Save("SeriesPropertyXErrorBarDemo.xlsx");
}
}
}
```
### See Also
* class [ErrorBar](../../errorbar/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
