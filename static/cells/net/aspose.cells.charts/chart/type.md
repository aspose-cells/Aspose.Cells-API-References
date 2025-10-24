##Chart.Type
Chart property. Gets or sets a charts type
## Chart.Type property
Gets or sets a chart's type.
```csharp
public ChartType Type { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for the chart
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["A2"].PutValue("A");
sheet.Cells["A3"].PutValue("B");
sheet.Cells["A4"].PutValue("C");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["B3"].PutValue(20);
sheet.Cells["B4"].PutValue(30);
// Add a radar chart
int chartIndex = sheet.Charts.Add(ChartType.Radar, 5, 0, 20, 8);
Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Demonstrate Type property usage
Console.WriteLine("Chart type is: " + chart.Type);
// Change chart type to Column
chart.Type = ChartType.Column;
Console.WriteLine("Chart type changed to: " + chart.Type);
}
}
}
```
### See Also
* enum [ChartType](../../charttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
