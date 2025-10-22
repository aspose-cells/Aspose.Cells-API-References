##ChartFrame.DefaultWidth
ChartFrame property. Represents width of default position in units of 1/4000 of the chart area
## ChartFrame.DefaultWidth property
Represents width of default position in units of 1/4000 of the chart area.
```csharp
[Obsolete("Use ChartFrame.DefaultWidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultWidth { get; }
```
### Remarks
NOTE: This member is now obsolete. Please use ChartFrame.DefaultWidthRatioToChart property, instead. DefaultWidth = (int)(DefaultWidthRatioToChart * 4000); This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class ChartFramePropertyDefaultWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Item1");
worksheet.Cells["A3"].PutValue("Item2");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Access the chart title (which inherits from ChartFrame)
Title title = chart.Title;
// Display the default width of the chart frame (title in this case)
Console.WriteLine("DefaultWidth of chart title: " + title.DefaultWidth);
// Note: DefaultWidth is read-only, so we cannot set it
// We can only read it to understand the default dimensions
// Demonstrate how this property affects the chart
Console.WriteLine("IsDefaultPosBeSet: " + title.IsDefaultPosBeSet);
Console.WriteLine("DefaultWidthRatioToChart: " + title.DefaultWidthRatioToChart);
// Save the workbook
workbook.Save("ChartFrameDefaultWidthDemo.xlsx");
}
}
}
```
### See Also
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
