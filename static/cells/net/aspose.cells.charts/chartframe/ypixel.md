##ChartFrame.YPixel
ChartFrame property. Gets or sets the y coordinate of the upper left corner in units of Pixel
## ChartFrame.YPixel property
Gets or sets the y coordinate of the upper left corner in units of Pixel.
```csharp
public virtual int YPixel { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartFramePropertyYPixelDemo
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
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access the chart title (which inherits from ChartFrame)
chart.Title.Text = "Sample Chart";
ChartFrame chartFrame = chart.Title;
// Display current YPixel value
Console.WriteLine("Current YPixel value: " + chartFrame.YPixel);
// Change the YPixel position of the chart title
chartFrame.YPixel = 50;
Console.WriteLine("New YPixel value: " + chartFrame.YPixel);
// Save the workbook
workbook.Save("ChartFrameYPixelDemo.xlsx");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
