##ChartTextFrame.IsAutomaticRotation
ChartTextFrame property. Indicates whether the text of the chart is automatically rotated
## ChartTextFrame.IsAutomaticRotation property
Indicates whether the text of the chart is automatically rotated.
```csharp
public bool IsAutomaticRotation { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartTextFramePropertyIsAutomaticRotationDemo
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
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Access value axis title and demonstrate IsAutomaticRotation
chart.ValueAxis.Title.Text = "Values";
bool isAutoRotate = chart.ValueAxis.Title.IsAutomaticRotation;
Console.WriteLine($"IsAutomaticRotation: {isAutoRotate}");
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
