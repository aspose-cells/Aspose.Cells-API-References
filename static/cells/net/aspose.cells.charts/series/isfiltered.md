##Series.IsFiltered
Series property. Indicates whether the series is selected or filtered.True represents this series is filtered and it will not be displayed on the chart
## Series.IsFiltered property
Indicates whether the series is selected or filtered.True represents this series is filtered, and it will not be displayed on the chart.
```csharp
public bool IsFiltered { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyIsFilteredDemo
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
worksheet.Cells["A5"].PutValue("D");
worksheet.Cells["B1"].PutValue("Series1");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["B5"].PutValue(40);
worksheet.Cells["C1"].PutValue("Series2");
worksheet.Cells["C2"].PutValue(15);
worksheet.Cells["C3"].PutValue(25);
worksheet.Cells["C4"].PutValue(35);
worksheet.Cells["C5"].PutValue(45);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B5", true);
chart.NSeries.Add("C2:C5", true);
chart.NSeries.CategoryData = "A2:A5";
// Demonstrate IsFiltered property
Console.WriteLine("Initial Series Count: " + chart.NSeries.Count);
// Filter the first series
chart.NSeries[0].IsFiltered = true;
Console.WriteLine("After filtering first series: " + chart.NSeries.Count);
// Filter the second series
chart.NSeries[0].IsFiltered = true;
Console.WriteLine("After filtering second series: " + chart.NSeries.Count);
// Save the workbook
workbook.Save("SeriesFilteredDemo_out.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
