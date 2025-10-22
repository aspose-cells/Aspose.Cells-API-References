##ChartTextFrame.IsAutoText
ChartTextFrame property. Indicates the text is auto generated
## ChartTextFrame.IsAutoText property
Indicates the text is auto generated.
```csharp
public virtual bool IsAutoText { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartTextFramePropertyIsAutoTextDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
// Set chart data
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Configure chart title
Aspose.Cells.Charts.ChartTextFrame title = chart.Title;
title.Text = "Custom Chart Title";
// Demonstrate IsAutoText property
title.IsAutoText = false; // Disable auto-generated text
// Save the workbook
workbook.Save("ChartTextFrame_IsAutoText_Demo.xlsx");
}
}
}
```
### See Also
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
