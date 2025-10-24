##Series.YErrorBar
Series property. Represents Y direction error bar of the series
## Series.YErrorBar property
Represents Y direction error bar of the series.
```csharp
public ErrorBar YErrorBar { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyYErrorBarDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("X");
sheet.Cells["A2"].PutValue(1);
sheet.Cells["A3"].PutValue(2);
sheet.Cells["A4"].PutValue(3);
sheet.Cells["B1"].PutValue("Y");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["B3"].PutValue(20);
sheet.Cells["B4"].PutValue(30);
// Create chart
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = sheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Set YErrorBar properties
ErrorBar errorBar = chart.NSeries[0].YErrorBar;
errorBar.Type = ErrorBarType.Percent;
errorBar.Amount = 5;
errorBar.DisplayType = ErrorBarDisplayType.Both;
// Save the workbook
workbook.Save("YErrorBarDemo.xlsx");
}
}
}
```
### See Also
* class [ErrorBar](../../errorbar/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
