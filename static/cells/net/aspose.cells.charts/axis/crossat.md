##Axis.CrossAt
Axis property. Represents the point on the value axis where the category axis crosses it
## Axis.CrossAt property
Represents the point on the value axis where the category axis crosses it.
```csharp
public double CrossAt { get; set; }
```
### Remarks
The number should be a integer when it applies to category axis. And the value must be between 1 and 31999.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyCrossAtDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["A5"].PutValue("D");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["B5"].PutValue(40);
// Add a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B5", true);
chart.NSeries.CategoryData = "A2:A5";
// Configure value axis
chart.ValueAxis.CrossAt = 15; // Cross at value 15
chart.ValueAxis.MinValue = 0;
chart.ValueAxis.MaxValue = 50;
// Configure category axis
chart.CategoryAxis.CrossAt = 2.5; // Cross between categories B and C
chart.CategoryAxis.TickLabelPosition = Aspose.Cells.Charts.TickLabelPositionType.Low;
// Save the workbook
workbook.Save("AxisCrossAtDemo.xlsx");
}
}
}
```
### See Also
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
