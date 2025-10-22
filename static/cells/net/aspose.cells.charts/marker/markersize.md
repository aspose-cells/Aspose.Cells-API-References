##Marker.MarkerSize
Marker property. Represents the marker size in unit of points. Applies to line chart scatter chart or radar chart
## Marker.MarkerSize property
Represents the marker size in unit of points. Applies to line chart, scatter chart, or radar chart.
```csharp
public int MarkerSize { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class MarkerPropertyMarkerSizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("X Values");
worksheet.Cells["B1"].PutValue("Y Values");
for (int i = 0; i < 10; i++)
{
worksheet.Cells[i + 1, 0].PutValue(i + 1);
worksheet.Cells[i + 1, 1].PutValue((i + 1) * 2);
}
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Add series - corrected method call
int seriesIndex = chart.NSeries.Add("B2:B11", true);
Series series = chart.NSeries[seriesIndex];
series.XValues = "A2:A11";
// Set marker properties
series.Marker.MarkerStyle = ChartMarkerType.Circle;
series.Marker.MarkerSize = 10; // Demonstrating MarkerSize property
series.Marker.ForegroundColor = Color.Red;
series.Marker.BackgroundColor = Color.Yellow;
// Save the workbook
workbook.Save("MarkerSizeDemo.xlsx");
}
}
}
```
### See Also
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
