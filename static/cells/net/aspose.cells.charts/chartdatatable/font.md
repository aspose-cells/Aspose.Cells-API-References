##ChartDataTable.Font
ChartDataTable property. Gets a Font object which represents the font setting of the specified chart data table
## ChartDataTable.Font property
Gets a `Font` object which represents the font setting of the specified chart data table.
```csharp
public Font Font { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ChartDataTablePropertyFontDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B1"].PutValue("Quantity");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(15);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Enable data table
chart.ShowDataTable = true;
// Get the data table object
ChartDataTable dataTable = chart.ChartDataTable;
// Customize data table font
dataTable.Font.Size = 14;
dataTable.Font.Color = Color.Red;
dataTable.Font.IsBold = true;
dataTable.Font.Name = "Arial";
// Save the workbook
workbook.Save("ChartDataTableFontDemo.xlsx");
}
}
}
```
### See Also
* class [Font](../../../aspose.cells/font/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
