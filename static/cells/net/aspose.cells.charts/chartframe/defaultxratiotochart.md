##ChartFrame.DefaultXRatioToChart
ChartFrame property. Represents x of default position in units of Fraction of the chart area
## ChartFrame.DefaultXRatioToChart property
Represents x of default position in units of Fraction of the chart area.
```csharp
public double DefaultXRatioToChart { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartFramePropertyDefaultXRatioToChartDemo
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
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the chart title frame
ChartFrame titleFrame = chart.Title;
// Display the current DefaultXRatioToChart value
Console.WriteLine("Default X Ratio To Chart (Title): " + titleFrame.DefaultXRatioToChart);
// Create a textbox in the chart
Aspose.Cells.Drawing.TextBox textBox = chart.Shapes.AddTextBoxInChart(50, 50, 200, 100);
// Get the shape properties of the textbox instead of trying to access ChartFrame directly
Console.WriteLine("Default X Ratio To Chart (TextBox): " + titleFrame.DefaultXRatioToChart);
// Demonstrate how these default ratios affect positioning
Console.WriteLine("Title X Position (Ratio): " + titleFrame.XRatioToChart);
Console.WriteLine("TextBox X Position (Ratio): " + titleFrame.XRatioToChart);
// Save the workbook
workbook.Save("ChartFrameDefaultXRatioToChartDemo.xlsx");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
