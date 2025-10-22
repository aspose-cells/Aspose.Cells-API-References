##Chart.PageSetup
Chart property. Represents the page setup description in this chart
## Chart.PageSetup property
Represents the page setup description in this chart.
```csharp
public PageSetup PageSetup { get; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyPageSetupDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and insert some data for the chart
Worksheet dataSheet = workbook.Worksheets[workbook.Worksheets.Add()];
dataSheet.Name = "DataSheet";
dataSheet.Cells["A1"].PutValue("Category");
dataSheet.Cells["A2"].PutValue("A");
dataSheet.Cells["A3"].PutValue("B");
dataSheet.Cells["A4"].PutValue("C");
dataSheet.Cells["B1"].PutValue("Value");
dataSheet.Cells["B2"].PutValue(10);
dataSheet.Cells["B3"].PutValue(20);
dataSheet.Cells["B4"].PutValue(30);
// Add a chart sheet
int chartSheetIndex = workbook.Worksheets.Add(SheetType.Chart);
Worksheet chartSheet = workbook.Worksheets[chartSheetIndex];
chartSheet.Name = "ChartSheet";
// Add a chart to the chart sheet
int chartIndex = chartSheet.Charts.Add(ChartType.Column, 0, 0, 800, 600);
Chart chart = chartSheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
// Access the PageSetup of the chart
PageSetup pageSetup = chart.PageSetup;
// Set page setup properties
pageSetup.Orientation = PageOrientationType.Landscape;
pageSetup.PaperSize = PaperSizeType.PaperA4;
pageSetup.Zoom = 90;
pageSetup.LeftMargin = 2.0;
pageSetup.RightMargin = 2.0;
pageSetup.TopMargin = 2.0;
pageSetup.BottomMargin = 2.0;
// Set header with text and image
byte[] imageData = File.ReadAllBytes("logo.png");
pageSetup.SetHeaderPicture(0, imageData);
pageSetup.SetHeader(0, "&G");
pageSetup.SetHeader(1, "Sales Report");
pageSetup.SetHeader(2, "&D");
// Set footer
pageSetup.SetFooter(0, "Page &P of &N");
// Save the workbook
workbook.Save("ChartPageSetupDemo.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../../../aspose.cells/pagesetup/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
