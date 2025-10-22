##Trendline.Name
Trendline property. Returns the name of the trendline
## Trendline.Name property
Returns the name of the trendline.
```csharp
public string Name { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TrendlinePropertyNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("X");
worksheet.Cells["B1"].PutValue("Y");
for (int i = 2; i <= 10; i++)
{
worksheet.Cells["A" + i].PutValue(i);
worksheet.Cells["B" + i].PutValue(i * 2);
}
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Add series to chart
chart.NSeries.Add("B2:B10", true);
chart.NSeries.CategoryData = "A2:A10";
// Add trendline and set its name
int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
trendline.Name = "My Custom Trendline";
// Save the workbook
workbook.Save("TrendlinePropertyNameDemo_out.xlsx");
}
}
}
```
### See Also
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
