##ChartTextFrame.DirectionType
ChartTextFrame property. Gets and sets the direction of text
## ChartTextFrame.DirectionType property
Gets and sets the direction of text.
```csharp
public virtual ChartTextDirectionType DirectionType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartTextFramePropertyDirectionTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
// Adding a worksheet returns its index, then we get the worksheet by index
int sheetIndex = workbook.Worksheets.Add();
Worksheet worksheet = workbook.Worksheets[sheetIndex];
// Add sample data
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["C1"].PutValue("Q1");
worksheet.Cells["C2"].PutValue("Q2");
worksheet.Cells["C3"].PutValue("Q3");
// Add chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
chart.NSeries.CategoryData = "C1:C3";
// Access and configure title
ChartTextFrame title = chart.Title;
title.Text = "Sample Chart";
// Demonstrate DirectionType property
title.DirectionType = ChartTextDirectionType.Vertical;
// Save the workbook
workbook.Save("ChartTextDirectionDemo.xlsx");
}
}
}
```
### See Also
* enum [ChartTextDirectionType](../../charttextdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
