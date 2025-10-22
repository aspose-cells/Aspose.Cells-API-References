##Chart.SetChartDataRange
Chart method. Specifies data range for a chart
## Chart.SetChartDataRange method
Specifies data range for a chart.
```csharp
public void SetChartDataRange(string area, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| area | String | Specifies values from which to plot the data series |
| isVertical | Boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartMethodSetChartDataRangeWithStringBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Series1");
worksheet.Cells["A2"].PutValue("Cat1");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("Cat2");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("Cat3");
worksheet.Cells["B4"].PutValue(30);
// Add chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.SetChartDataRange("A1:B4", true);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
