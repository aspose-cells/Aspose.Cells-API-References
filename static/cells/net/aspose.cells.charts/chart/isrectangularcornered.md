##Chart.IsRectangularCornered
Chart property. Gets or sets a value indicating whether the chart area is rectangular cornered. Default is true
## Chart.IsRectangularCornered property
Gets or sets a value indicating whether the chart area is rectangular cornered. Default is true.
```csharp
public bool IsRectangularCornered { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyIsRectangularCorneredDemo
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
// Add a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Demonstrate IsRectangularCornered property
Console.WriteLine("Default IsRectangularCornered: " + chart.IsRectangularCornered);
// Set to true to make chart corners rectangular
chart.IsRectangularCornered = true;
Console.WriteLine("After setting IsRectangularCornered to true: " + chart.IsRectangularCornered);
// Save the workbook
workbook.Save("ChartPropertyIsRectangularCorneredDemo_out.xlsx");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
