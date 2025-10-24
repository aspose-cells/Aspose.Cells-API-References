##Chart.HeightPercent
Chart property. Returns or sets the height of a 3D chart as a percentage of the chart width between 5 and 500 percent
## Chart.HeightPercent property
Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent).
```csharp
public int HeightPercent { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyHeightPercentDemo
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
// Add a 3D column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Set HeightPercent property (controls the height of 3D chart as percentage of chart width)
chart.HeightPercent = 150; // 150% of chart width
// Save the workbook
workbook.Save("ChartHeightPercentDemo.xlsx");
Console.WriteLine("Chart with HeightPercent 150% created successfully.");
}
}
}
```
### See Also
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
