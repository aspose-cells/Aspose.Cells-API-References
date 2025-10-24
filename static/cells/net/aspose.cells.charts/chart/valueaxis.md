##Chart.ValueAxis
Chart property. Gets the charts Y axis
## Chart.ValueAxis property
Gets the chart's Y axis.
```csharp
public Axis ValueAxis { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyValueAxisDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(100000000);
worksheet.Cells["B3"].PutValue(200000000);
worksheet.Cells["B4"].PutValue(300000000);
// Add a chart and set its data range
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Configure ValueAxis properties
chart.ValueAxis.DisplayUnit = DisplayUnitType.HundredMillions;
chart.ValueAxis.Title.Text = "Values (in 100 millions)";
chart.ValueAxis.MajorUnit = 1;
// Save the workbook
workbook.Save("ChartPropertyValueAxisDemo.xlsx");
}
}
}
```
### See Also
* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
