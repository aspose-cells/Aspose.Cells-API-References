##Trendline.LegendEntry
Trendline property. Gets the legend entry according to this trendline
## Trendline.LegendEntry property
Gets the legend entry according to this trendline
```csharp
public LegendEntry LegendEntry { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
using System.Drawing;
public class TrendlinePropertyLegendEntryDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("X");
worksheet.Cells["B1"].PutValue("Y");
for (int i = 2; i <= 5; i++)
{
worksheet.Cells[$"A{i}"].PutValue(i);
worksheet.Cells[$"B{i}"].PutValue(i * 2);
}
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B5", true);
chart.NSeries.CategoryData = "A2:A5";
// Fix: Get trendline index first then retrieve the trendline object
int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
LegendEntry legendEntry = trendline.LegendEntry;
Console.WriteLine("Initial LegendEntry.IsDeleted: " + legendEntry.IsDeleted);
Console.WriteLine("Initial Font Color: " + legendEntry.Font.Color);
legendEntry.IsDeleted = true;
legendEntry.Font.Size = 14;
legendEntry.Font.Color = Color.Red;
workbook.Save("TrendlineLegendEntryDemo.xlsx");
}
}
}
```
### See Also
* class [LegendEntry](../../legendentry/)
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
