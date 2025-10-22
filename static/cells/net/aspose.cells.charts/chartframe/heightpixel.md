##ChartFrame.HeightPixel
ChartFrame property. Gets or sets the height of frame in units of Pixel
## ChartFrame.HeightPixel property
Gets or sets the height of frame in units of Pixel.
```csharp
public virtual int HeightPixel { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartFramePropertyHeightPixelDemo
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
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access the chart title (which is a ChartFrame)
ChartFrame chartTitle = chart.Title;
// Display current height in pixels
Console.WriteLine("Current title height: " + chartTitle.HeightPixel + " pixels");
// Set a new height for the title
chartTitle.HeightPixel = 40;
Console.WriteLine("New title height: " + chartTitle.HeightPixel + " pixels");
// Access the legend (another ChartFrame)
ChartFrame legend = chart.Legend;
// Display and modify legend height
Console.WriteLine("Current legend height: " + legend.HeightPixel + " pixels");
legend.HeightPixel = 60;
Console.WriteLine("New legend height: " + legend.HeightPixel + " pixels");
// Save the workbook
workbook.Save("ChartFrameHeightPixelDemo.xlsx");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
