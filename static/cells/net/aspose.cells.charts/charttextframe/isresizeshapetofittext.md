##ChartTextFrame.IsResizeShapeToFitText
ChartTextFrame property. Gets or sets whether a shape should be autofit to fully contain the text described within it. Autofitting is when text within a shape is scaled in order to contain all the text inside
## ChartTextFrame.IsResizeShapeToFitText property
Gets or sets whether a shape should be auto-fit to fully contain the text described within it. Auto-fitting is when text within a shape is scaled in order to contain all the text inside.
```csharp
public bool IsResizeShapeToFitText { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class ChartTextFramePropertyIsResizeShapeToFitTextDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook(FileFormatType.Xlsx);
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category 1");
worksheet.Cells["A2"].PutValue("Category 2");
worksheet.Cells["A3"].PutValue("Category 3");
worksheet.Cells["B1"].PutValue(10);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(30);
// Add a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Set series data
chart.NSeries.Add("B1:B3", true);
chart.NSeries.CategoryData = "A1:A3";
// Access data labels
DataLabels dataLabels = chart.NSeries[0].DataLabels;
dataLabels.ShowValue = true;
dataLabels.Position = LabelPositionType.Center;
// Demonstrate IsResizeShapeToFitText property
foreach (ChartPoint point in chart.NSeries[0].Points)
{
// Disable auto-resizing of shape to fit text
point.DataLabels.IsResizeShapeToFitText = false;
// Set custom width that's smaller than text would normally require
point.DataLabels.Width = 50;
}
// Save the workbook
workbook.Save("ChartTextFramePropertyIsResizeShapeToFitTextDemo.xlsx");
}
}
}
```
### See Also
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
