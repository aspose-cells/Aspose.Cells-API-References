##ChartDataTable.ShowLegendKey
ChartDataTable property. True if the data label legend key is visible
## ChartDataTable.ShowLegendKey property
True if the data label legend key is visible.
```csharp
public bool ShowLegendKey { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartDataTablePropertyShowLegendKeyDemo
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
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Enable data table with legend key
chart.ShowDataTable = true;
// Access DataTable through Chart's properties
if (chart.ChartDataTable != null)
{
chart.ChartDataTable.ShowLegendKey = true;
}
// Save the workbook
workbook.Save("ChartDataTableShowLegendKeyDemo.xlsx");
Console.WriteLine("Chart created with ShowLegendKey enabled in data table.");
}
}
}
```
### See Also
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
