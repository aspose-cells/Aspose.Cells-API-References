##Title.IsVisible
Title property. Represents whether the title is visible
## Title.IsVisible property
Represents whether the title is visible.
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
public class TitlePropertyIsVisibleDemo
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
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Demonstrate IsVisible property
chart.Title.IsVisible = true;
chart.Title.Text = "Sample Chart";
chart.CategoryAxis.Title.IsVisible = true;
chart.CategoryAxis.Title.Text = "Categories";
chart.ValueAxis.Title.IsVisible = true;
chart.ValueAxis.Title.Text = "Values";
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
