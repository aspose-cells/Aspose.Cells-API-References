##Chart.IsReferedByChart
Chart method. Returns whether the cell refered by the chart
## Chart.IsReferedByChart method
Returns whether the cell refered by the chart.
```csharp
[Obsolete("Use Chart.IsCellReferedByChart(int,int,int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsReferedByChart(int rowIndex, int columnIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | The row index |
| columnIndex | Int32 | The column index |
### Remarks
NOTE: This method is now obsolete. Instead, please use IsCellReferedByChart(int,int,int) method. This method will be removed 12 months later since April 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartMethodIsReferedByChartWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Fruit");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["B1"].PutValue("Quantity");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(15);
worksheet.Cells["B4"].PutValue(20);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.SetChartDataRange("A1:B4", true);
try
{
// Check if cell B2 (row 1, column 1) is referred by the chart
bool isReferred = chart.IsReferedByChart(1, 1);
Console.WriteLine($"Is cell B2 referred by the chart? {isReferred}");
// Check a cell that's not in the chart data range
bool isNotReferred = chart.IsReferedByChart(10, 10);
Console.WriteLine($"Is cell K11 referred by the chart? {isNotReferred}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing IsReferedByChart method: {ex.Message}");
}
// Save the workbook
workbook.Save("ChartMethodIsReferedByChartWithInt32Int32Demo.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
