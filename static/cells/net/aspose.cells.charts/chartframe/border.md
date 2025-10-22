##ChartFrame.Border
ChartFrame property. Gets the border
## ChartFrame.Border property
Gets the [`border`](../../../aspose.cells.drawing/line/).
```csharp
public virtual Line Border { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ChartFramePropertyBorderDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B4"].PutValue(30);
// Add a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access chart title
chart.Title.Text = "Chart Title with Custom Border";
ChartFrame title = chart.Title;
// Configure border properties
Line border = title.Border;
border.Color = System.Drawing.Color.Red;
border.Style = LineType.Solid;
border.Weight = WeightType.MediumLine;
border.Transparency = 0.3;
border.DashType = MsoLineDashStyle.Solid;
// Save the result
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Line](../../../aspose.cells.drawing/line/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
