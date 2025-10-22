##Chart.DepthPercent
Chart property. Represents the depth of a 3D chart as a percentage of the chart width between 20 and 2000 percent
## Chart.DepthPercent property
Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent).
```csharp
public int DepthPercent { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyDepthPercentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Q1");
worksheet.Cells["A3"].PutValue("Q2");
worksheet.Cells["A4"].PutValue("Q3");
worksheet.Cells["B1"].PutValue("Series1");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(300);
worksheet.Cells["C1"].PutValue("Series2");
worksheet.Cells["C2"].PutValue(150);
worksheet.Cells["C3"].PutValue(250);
worksheet.Cells["C4"].PutValue(350);
// Add a 3D column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:C4", true);
chart.NSeries.CategoryData = "A2:A4";
// Set DepthPercent property (controls the depth of 3D chart as percentage of chart width)
chart.DepthPercent = 150; // 150% depth
// Save the workbook
workbook.Save("ChartDepthPercentDemo.xlsx");
Console.WriteLine("Chart with DepthPercent 150% created successfully.");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
