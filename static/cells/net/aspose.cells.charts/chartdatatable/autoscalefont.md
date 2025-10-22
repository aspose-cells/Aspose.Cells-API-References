##ChartDataTable.AutoScaleFont
ChartDataTable property. True if the text in the object changes font size when the object size changes. The default value is True
## ChartDataTable.AutoScaleFont property
True if the text in the object changes font size when the object size changes. The default value is True.
```csharp
public bool AutoScaleFont { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartDataTablePropertyAutoScaleFontDemo
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
// Enable data table
chart.ShowDataTable = true;
// Access chart data table properties
// Correct way to get ChartDataTable when ShowDataTable is true
ChartDataTable dataTable = chart.ChartDataTable;
// Demonstrate AutoScaleFont property
dataTable.AutoScaleFont = false; // Disable auto-scaling
Console.WriteLine("AutoScaleFont (false): " + dataTable.AutoScaleFont);
dataTable.AutoScaleFont = true; // Enable auto-scaling
Console.WriteLine("AutoScaleFont (true): " + dataTable.AutoScaleFont);
// Save the workbook
workbook.Save("ChartDataTableAutoScaleFontDemo.xlsx");
}
}
}
```
### See Also
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
