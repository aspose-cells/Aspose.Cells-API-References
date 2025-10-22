##ChartShape.Chart
ChartShape property. Returns a Chart object that represents the chart contained in the object
## ChartShape.Chart property
Returns a Chart object that represents the chart contained in the object.
```csharp
public Chart Chart { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
public class ChartShapePropertyChartDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Fruits");
worksheet.Cells["A3"].PutValue("Vegetables");
worksheet.Cells["A4"].PutValue("Grains");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(50);
worksheet.Cells["B3"].PutValue(30);
worksheet.Cells["B4"].PutValue(20);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the ChartShape instance
ChartShape chartShape = (ChartShape)chart.ChartObject;
// Access the Chart property (read-only)
Chart accessedChart = chartShape.Chart;
// Display chart properties
Console.WriteLine("Chart Name: " + accessedChart.Name);
Console.WriteLine("Chart Type: " + accessedChart.Type);
Console.WriteLine("Show Legend: " + accessedChart.ShowLegend);
// Modify chart properties through the Chart object
accessedChart.Name = "Sales Chart";
accessedChart.ShowLegend = false;
accessedChart.Title.Text = "Product Sales Distribution";
// Change chart type
accessedChart.Type = ChartType.Pie;
// Save the result
workbook.Save("ChartShapePropertyChartDemo.xlsx");
}
}
}
```
### See Also
* class [Chart](../../../aspose.cells.charts/chart/)
* class [ChartShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
