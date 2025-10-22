##Series.IsAutoSplit
Series property. Indicates whether the threshold value is automatic
## Series.IsAutoSplit property
Indicates whether the threshold value is automatic.
```csharp
public bool IsAutoSplit { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyIsAutoSplitDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["A5"].PutValue("Grape");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["B5"].PutValue(40);
// Add a pie chart
int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B5", true);
chart.NSeries.CategoryData = "A2:A5";
// Access the first series and demonstrate IsAutoSplit property
Series series = chart.NSeries[0];
bool isAutoSplit = series.IsAutoSplit; // Get the value instead of setting it
series.SplitValue = 25; // Split at value 25
Console.WriteLine($"IsAutoSplit value: {isAutoSplit}");
// Save the workbook
workbook.Save("SeriesPropertyIsAutoSplitDemo_out.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
