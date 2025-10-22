##Chart.SwitchRowColumn
Chart method. Switches row/column
## Chart.SwitchRowColumn method
Switches row/column.
```csharp
public bool SwitchRowColumn()
```
### Return Value
False means switching row/column fails.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartMethodSwitchRowColumnDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Series 1");
worksheet.Cells["C1"].PutValue("Series 2");
worksheet.Cells["A2"].PutValue("Item 1");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["C2"].PutValue(150);
worksheet.Cells["A3"].PutValue("Item 2");
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["C3"].PutValue(250);
worksheet.Cells["A4"].PutValue("Item 3");
worksheet.Cells["B4"].PutValue(300);
worksheet.Cells["C4"].PutValue(350);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.SetChartDataRange("A1:C4", true);
// Show original series values
Console.WriteLine("Before SwitchRowColumn:");
Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
// Switch row/column
chart.SwitchRowColumn();
// Show series values after switching
Console.WriteLine("\nAfter SwitchRowColumn:");
Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
// Save the workbook
workbook.Save("SwitchRowColumnDemo.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
