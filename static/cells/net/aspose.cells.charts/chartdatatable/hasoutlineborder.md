##ChartDataTable.HasOutlineBorder
ChartDataTable property. True if the chart data table has outline borders
## ChartDataTable.HasOutlineBorder property
True if the chart data table has outline borders
```csharp
public bool HasOutlineBorder { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartDataTablePropertyHasOutlineBorderDemo
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
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Show data table and get ChartDataTable object
chart.ShowDataTable = true;
ChartDataTable dataTable = chart.ChartDataTable;
// Demonstrate HasOutlineBorder property
dataTable.HasOutlineBorder = true; // Enable outline border
Console.WriteLine("DataTable HasOutlineBorder: " + dataTable.HasOutlineBorder);
// Save the workbook
workbook.Save("ChartDataTableHasOutlineBorderDemo.xlsx");
}
}
}
```
### See Also
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
