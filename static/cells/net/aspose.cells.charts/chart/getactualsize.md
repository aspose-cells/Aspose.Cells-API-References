##Chart.GetActualSize
Chart method. Gets actual size of chart in unit of pixels
## Chart.GetActualSize method
Gets actual size of chart in unit of pixels.
```csharp
public int[] GetActualSize()
```
### Return Value
Actual size in an array(width and height). [0] is width; [1] is height.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartMethodGetActualSizeDemo
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
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.SetChartDataRange("A1:B4", true);
try
{
// Call the GetActualSize method
int[] actualSize = chart.GetActualSize();
// Display the result
Console.WriteLine($"Actual chart size - Width: {actualSize[0]}px, Height: {actualSize[1]}px");
// Show the effect by resizing the chart object
chart.ChartObject.Width = actualSize[0];
chart.ChartObject.Height = actualSize[1];
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetActualSize method: {ex.Message}");
}
// Save the result
workbook.Save("ChartMethodGetActualSizeDemo.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
