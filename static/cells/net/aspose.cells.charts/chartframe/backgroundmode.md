##ChartFrame.BackgroundMode
ChartFrame property. Gets and sets the display mode of the background
## ChartFrame.BackgroundMode property
Gets and sets the display mode of the background
```csharp
public BackgroundMode BackgroundMode { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartFramePropertyBackgroundModeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["A2"].PutValue("Apple");
sheet.Cells["A3"].PutValue("Orange");
sheet.Cells["A4"].PutValue("Banana");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["B2"].PutValue(50);
sheet.Cells["B3"].PutValue(30);
sheet.Cells["B4"].PutValue(20);
// Add a chart
int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
// Set chart data
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Demonstrate BackgroundMode property
chart.ChartArea.BackgroundMode = Aspose.Cells.Charts.BackgroundMode.Transparent;
chart.PlotArea.BackgroundMode = Aspose.Cells.Charts.BackgroundMode.Automatic;
// Save the workbook
workbook.Save("ChartBackgroundModeDemo.xlsx");
}
}
}
```
### See Also
* enum [BackgroundMode](../../backgroundmode/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
