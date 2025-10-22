##Axis.IsVisible
Axis property. Represents if the axis is visible
## Axis.IsVisible property
Represents if the axis is visible.
```csharp
public bool IsVisible { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyIsVisibleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B4"].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Add a secondary axis series
chart.NSeries.Add("B2:B4", true);
chart.NSeries[1].PlotOnSecondAxis = true;
// Demonstrate IsVisible property
Console.WriteLine("Secondary Value Axis Visible: " + chart.SecondValueAxis.IsVisible);
// Hide the secondary axis
chart.SecondValueAxis.IsVisible = false;
Console.WriteLine("After setting to false - Secondary Value Axis Visible: " + chart.SecondValueAxis.IsVisible);
// Save the workbook
workbook.Save("AxisIsVisibleDemo.xlsx");
}
}
}
```
### See Also
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
