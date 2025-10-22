##Trendline.Type
Trendline property. Returns the trendline type
## Trendline.Type property
Returns the trendline type.
```csharp
public TrendlineType Type { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TrendlinePropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("X");
sheet.Cells["A2"].PutValue(1);
sheet.Cells["A3"].PutValue(2);
sheet.Cells["A4"].PutValue(3);
sheet.Cells["A5"].PutValue(4);
sheet.Cells["B1"].PutValue("Y");
sheet.Cells["B2"].PutValue(2);
sheet.Cells["B3"].PutValue(4);
sheet.Cells["B4"].PutValue(8);
sheet.Cells["B5"].PutValue(16);
// Add a chart
int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 8);
Chart chart = sheet.Charts[chartIndex];
// Add series
chart.NSeries.Add("A2:A5", true);
chart.NSeries[0].XValues = "B2:B5";
// Add exponential trendline
int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);
Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
// Demonstrate Type property usage
Console.WriteLine("Trendline type: " + trendline.Type);
// Save the workbook
workbook.Save("TrendlinePropertyTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [TrendlineType](../../trendlinetype/)
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
