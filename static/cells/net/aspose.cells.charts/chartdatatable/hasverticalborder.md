##ChartDataTable.HasVerticalBorder
ChartDataTable property. True if the chart data table has vertical cell borders
## ChartDataTable.HasVerticalBorder property
True if the chart data table has vertical cell borders
```csharp
public bool HasVerticalBorder { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartDataTablePropertyHasVerticalBorderDemo
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
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Show data table
chart.ShowDataTable = true;
// Access the data table through ChartDataTable property
ChartDataTable dataTable = chart.ChartDataTable;
// Demonstrate HasVerticalBorder property
Console.WriteLine("Initial HasVerticalBorder value: " + dataTable.HasVerticalBorder);
// Toggle vertical borders
dataTable.HasVerticalBorder = true;
Console.WriteLine("After setting HasVerticalBorder to true: " + dataTable.HasVerticalBorder);
dataTable.HasVerticalBorder = false;
Console.WriteLine("After setting HasVerticalBorder to false: " + dataTable.HasVerticalBorder);
// Save the workbook
workbook.Save("ChartDataTable_HasVerticalBorderDemo.xlsx");
}
}
}
```
### See Also
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
