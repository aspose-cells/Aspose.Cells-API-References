##Chart.IsCellReferedByChart
Chart method. Returns whether the cell refered by the chart
## Chart.IsCellReferedByChart method
Returns whether the cell refered by the chart.
```csharp
public bool IsCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | The sheet Index.-1 means the worksheet which contains current chart. |
| rowIndex | Int32 | The row index |
| columnIndex | Int32 | The column index |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartMethodIsCellReferedByChartWithInt32Int32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
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
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Check if cell is referred by chart
bool isReferred = chart.IsCellReferedByChart(0, 1, 0); // Check if B2 is referred
Console.WriteLine("Is cell B2 referred by chart: " + isReferred);
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
