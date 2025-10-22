##Chart.ShowLegend
Chart property. Gets or sets a value indicating whether the chart legend will be displayed. Default is true
## Chart.ShowLegend property
Gets or sets a value indicating whether the chart legend will be displayed. Default is true.
```csharp
public bool ShowLegend { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyShowLegendDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Item");
sheet.Cells["A2"].PutValue("Apple");
sheet.Cells["A3"].PutValue("Orange");
sheet.Cells["A4"].PutValue("Banana");
sheet.Cells["B1"].PutValue("Quantity");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["B3"].PutValue(20);
sheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Show legend by default (true)
Console.WriteLine("Legend initially visible: " + chart.ShowLegend);
// Hide the legend
chart.ShowLegend = false;
Console.WriteLine("Legend after setting to false: " + chart.ShowLegend);
// Save the workbook
workbook.Save("ChartLegendExample.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
