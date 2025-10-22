##Series.LegendEntry
Series property. Gets the legend entry according to this series
## Series.LegendEntry property
Gets the legend entry according to this series.
```csharp
public LegendEntry LegendEntry { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyLegendEntryDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the first series
Series series = chart.NSeries[0];
// Demonstrate LegendEntry functionality
Console.WriteLine("LegendEntry.IsDeleted before: " + series.LegendEntry.IsDeleted);
series.LegendEntry.IsDeleted = true;
Console.WriteLine("LegendEntry.IsDeleted after setting to true: " + series.LegendEntry.IsDeleted);
series.LegendEntry.IsDeleted = false;
Console.WriteLine("LegendEntry.IsDeleted after setting to false: " + series.LegendEntry.IsDeleted);
// Save the workbook
workbook.Save("SeriesPropertyLegendEntryDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [LegendEntry](../../legendentry/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
