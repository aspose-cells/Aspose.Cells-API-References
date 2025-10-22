##ChartDataTable.Border
ChartDataTable property. Returns a Border object that represents the border of the object
## ChartDataTable.Border property
Returns a Border object that represents the border of the object
```csharp
public Line Border { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ChartDataTablePropertyBorderDemo
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
// Add a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Show data table
chart.ShowDataTable = true;
ChartDataTable dataTable = chart.ChartDataTable;
// Configure border properties
Line border = dataTable.Border;
border.Color = System.Drawing.Color.Blue;
border.Style = LineType.Solid;
border.Weight = WeightType.MediumLine;
border.DashType = MsoLineDashStyle.Solid;
// Configure table borders visibility
dataTable.HasHorizontalBorder = true;
dataTable.HasVerticalBorder = true;
dataTable.HasOutlineBorder = true;
// Save the workbook
workbook.Save("ChartDataTableBorderDemo.xlsx");
}
}
}
```
### See Also
* class [Line](../../../aspose.cells.drawing/line/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
