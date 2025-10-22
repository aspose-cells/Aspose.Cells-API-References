##ChartFrame.AutoScaleFont
ChartFrame property. True if the text in the object changes font size when the object size changes. The default value is True
## ChartFrame.AutoScaleFont property
True if the text in the object changes font size when the object size changes. The default value is True.
```csharp
public virtual bool AutoScaleFont { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartFramePropertyAutoScaleFontDemo
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
// Access the chart title
chart.Title.Text = "Sample Chart";
// Demonstrate AutoScaleFont property
chart.Title.AutoScaleFont = true;
Console.WriteLine("Chart title AutoScaleFont is set to: " + chart.Title.AutoScaleFont);
// Save the workbook
workbook.Save("ChartFrameAutoScaleFontDemo.xlsx");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
