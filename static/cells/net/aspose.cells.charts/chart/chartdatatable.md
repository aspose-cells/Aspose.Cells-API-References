##Chart.ChartDataTable
Chart property. Represents the chart data table
## Chart.ChartDataTable property
Represents the chart data table.
```csharp
public ChartDataTable ChartDataTable { get; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ChartPropertyChartDataTableDemo
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
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(300);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("=Sheet1!$B$2:$B$4", true);
chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$4";
// Enable and customize the data table
chart.ShowDataTable = true;
ChartDataTable dataTable = chart.ChartDataTable;
// Set data table properties
dataTable.ShowLegendKey = true;
dataTable.HasBorderHorizontal = true;
dataTable.HasBorderVertical = true;
dataTable.HasBorderOutline = true;
dataTable.AutoScaleFont = true;
dataTable.BackgroundMode = BackgroundMode.Opaque;
// Customize data table font
dataTable.Font.Name = "Arial";
dataTable.Font.Size = 10;
dataTable.Font.Color = Color.Blue;
dataTable.Font.IsBold = true;
// Customize data table borders
dataTable.Border.Color = Color.Red;
dataTable.Border.Style = LineType.Dash;
dataTable.Border.Weight = WeightType.MediumLine;
// Save the workbook
workbook.Save("ChartDataTableDemo.xlsx");
}
}
}
```
### See Also
* class [ChartDataTable](../../chartdatatable/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
