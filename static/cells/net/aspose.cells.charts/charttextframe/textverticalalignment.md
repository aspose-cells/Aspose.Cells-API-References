##ChartTextFrame.TextVerticalAlignment
ChartTextFrame property. Gets or sets the text vertical alignment of text
## ChartTextFrame.TextVerticalAlignment property
Gets or sets the text vertical alignment of text.
```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartTextFramePropertyTextVerticalAlignmentDemo
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
// Add a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
// Set the title and configure vertical alignment
chart.Title.Text = "Sample Chart";
chart.Title.TextVerticalAlignment = TextAlignmentType.Top;
// Configure the display unit label
chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
chart.ValueAxis.DisplayUnitLabel.Text = "Values in Hundreds";
chart.ValueAxis.DisplayUnitLabel.TextVerticalAlignment = TextAlignmentType.Center;
// Save the workbook
workbook.Save("ChartTextVerticalAlignmentDemo.xlsx");
Console.WriteLine("Demo executed successfully. Output file: ChartTextVerticalAlignmentDemo.xlsx");
}
}
}
```
### See Also
* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
