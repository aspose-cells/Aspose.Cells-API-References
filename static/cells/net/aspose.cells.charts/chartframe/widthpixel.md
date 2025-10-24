##ChartFrame.WidthPixel
ChartFrame property. Gets or sets the width of frame in units of Pixel
## ChartFrame.WidthPixel property
Gets or sets the width of frame in units of Pixel.
```csharp
public virtual int WidthPixel { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartFramePropertyWidthPixelDemo
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
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access the chart title (which inherits from ChartFrame)
chart.Title.Text = "Sample Chart";
// Display current WidthPixel value of the chart title
Console.WriteLine("Current Title WidthPixel: " + chart.Title.WidthPixel);
// Set a new width for the chart title in pixels
chart.Title.WidthPixel = 300;
// Display the new WidthPixel value
Console.WriteLine("New Title WidthPixel: " + chart.Title.WidthPixel);
// Save the workbook
workbook.Save("ChartFrameWidthPixelDemo.xlsx");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
