##Trendline.IsNameAuto
Trendline property. Returns if Microsoft Excel automatically determines the name of the trendline
## Trendline.IsNameAuto property
Returns if Microsoft Excel automatically determines the name of the trendline.
```csharp
public bool IsNameAuto { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TrendlinePropertyIsNameAutoDemo
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
// Add trendline - modified to ensure proper Trendline object creation
int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
// Demonstrate IsNameAuto property
Console.WriteLine("Initial IsNameAuto value: " + trendline.IsNameAuto);
// Set custom name (disables auto naming)
trendline.Name = "Custom Trendline Name";
Console.WriteLine("After setting custom name, IsNameAuto: " + trendline.IsNameAuto);
// Reset to auto name
trendline.IsNameAuto = true;
Console.WriteLine("After setting IsNameAuto=true, Name: " + trendline.Name);
}
}
}
```
### See Also
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
