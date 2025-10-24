##ChartTextFrame.TextHorizontalAlignment
ChartTextFrame property. Gets and sets the text horizontal alignment
## ChartTextFrame.TextHorizontalAlignment property
Gets and sets the text horizontal alignment.
```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartTextFramePropertyTextHorizontalAlignmentDemo
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
// Add a chart and set its data range
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the chart title and set properties
Title title = chart.Title;
title.Text = "Sample Chart Title";
// Demonstrate TextHorizontalAlignment property
title.TextHorizontalAlignment = TextAlignmentType.Center;
Console.WriteLine("Title horizontal alignment set to: " + title.TextHorizontalAlignment);
// Save the workbook
workbook.Save("ChartTextHorizontalAlignmentDemo.xlsx");
}
}
}
```
### See Also
* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
