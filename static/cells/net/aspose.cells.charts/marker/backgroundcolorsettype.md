##Marker.BackgroundColorSetType
Marker property. Gets or sets the marker background color set type
## Marker.BackgroundColorSetType property
Gets or sets the marker background color set type.
```csharp
public FormattingType BackgroundColorSetType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class MarkerPropertyBackgroundColorSetTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add series
int seriesIndex = chart.NSeries.Add("A1:B3", true);
Series series = chart.NSeries[seriesIndex];
// Configure marker properties
series.Marker.MarkerStyle = ChartMarkerType.Circle;
series.Marker.BackgroundColorSetType = FormattingType.Automatic;
series.Marker.BackgroundColor = System.Drawing.Color.Yellow;
// Save the workbook
workbook.Save("MarkerBackgroundColorSetTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [FormattingType](../../formattingtype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
