##Axis.Title
Axis property. Gets the axis title
## Axis.Title property
Gets the axis' title.
```csharp
public Title Title { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyTitleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Configure titles
chart.Title.Text = "Sample Chart";
chart.Title.IsVisible = true;
chart.Title.Font.Name = "Aktiv Grotesk";
chart.Title.Font.Size = 14;
// Configure axis titles
chart.CategoryAxis.Title.Text = "Categories";
chart.CategoryAxis.Title.IsVisible = true;
chart.CategoryAxis.Title.Font.Name = "Arial";
chart.ValueAxis.Title.Text = "Values";
chart.ValueAxis.Title.IsVisible = true;
chart.ValueAxis.Title.Font.Name = "Aktiv Grotesk";
// Save the workbook
workbook.Save("AxisPropertyTitleDemo_Output.xlsx");
}
}
}
```
### See Also
* class [Title](../../title/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
