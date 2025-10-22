##Chart.RightAngleAxes
Chart property. True if the chart axes are at right angles. Applies only for 3D chartsexcept Column3D and 3D Pie Charts
## Chart.RightAngleAxes property
True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts).
```csharp
public bool RightAngleAxes { get; set; }
```
### Remarks
If this property is True, the Perspective property is ignored.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyRightAngleAxesDemo
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
worksheet.Cells["B3"].PutValue(25);
worksheet.Cells["B4"].PutValue(35);
// Add a 3D column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Demonstrate RightAngleAxes property
chart.RightAngleAxes = true;
Console.WriteLine("RightAngleAxes is set to: " + chart.RightAngleAxes);
// Save the workbook
workbook.Save("RightAngleAxesDemo.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
