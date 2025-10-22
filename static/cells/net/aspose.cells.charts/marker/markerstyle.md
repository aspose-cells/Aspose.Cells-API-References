##Marker.MarkerStyle
Marker property. Represents the marker style. Applies to line chart scatter chart or radar chart
## Marker.MarkerStyle property
Represents the marker style. Applies to line chart, scatter chart, or radar chart.
```csharp
public ChartMarkerType MarkerStyle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class MarkerPropertyMarkerStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("X");
sheet.Cells["A2"].PutValue(1);
sheet.Cells["A3"].PutValue(2);
sheet.Cells["A4"].PutValue(3);
sheet.Cells["B1"].PutValue("Y");
sheet.Cells["B2"].PutValue(4);
sheet.Cells["B3"].PutValue(5);
sheet.Cells["B4"].PutValue(6);
// Add a chart
int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
Chart chart = sheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("A2:A4", true);
chart.NSeries.CategoryData = "B2:B4";
// Set marker style for the first series
chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Circle;
chart.NSeries[0].Marker.ForegroundColor = System.Drawing.Color.Blue;
chart.NSeries[0].Marker.BackgroundColor = System.Drawing.Color.White;
chart.NSeries[0].Marker.MarkerSize = 10;
// Save the workbook
workbook.Save("MarkerStyleDemo.xlsx");
}
}
}
```
### See Also
* enum [ChartMarkerType](../../chartmarkertype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
