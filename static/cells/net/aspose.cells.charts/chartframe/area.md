##ChartFrame.Area
ChartFrame property. Gets the area
## ChartFrame.Area property
Gets the `area`.
```csharp
public virtual Area Area { get; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ChartFramePropertyAreaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for the chart
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["A2"].PutValue("A");
sheet.Cells["A3"].PutValue("B");
sheet.Cells["A4"].PutValue("C");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["B3"].PutValue(20);
sheet.Cells["B4"].PutValue(30);
// Add a chart to the worksheet
int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = sheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access the chart area
ChartArea chartArea = chart.ChartArea;
// Demonstrate Area property functionality
Area area = chartArea.Area;
Console.WriteLine("Original Formatting: " + area.Formatting);
// Modify area properties
area.Formatting = FormattingType.Custom;
area.BackgroundColor = Color.LightBlue;
area.ForegroundColor = Color.DarkBlue;
area.Transparency = 0.3;
area.InvertIfNegative = true;
// Save the workbook
workbook.Save("ChartFramePropertyAreaDemo.xlsx");
}
}
}
```
### See Also
* class [Area](../../../aspose.cells.drawing/area/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
