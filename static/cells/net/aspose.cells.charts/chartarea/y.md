##ChartArea.Y
ChartArea property. Gets or gets the vertical offset from its upper left corner row in units of 1/4000 of the chart area
## ChartArea.Y property
Gets or gets the vertical offset from its upper left corner row, in units of 1/4000 of the chart area.
```csharp
[Obsolete("Use ChartArea.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Y { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Please use ChartArea.YRatioToChart property, instead. Y = YRatioToChart * 4000; This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartAreaPropertyYDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
// Add chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
// Configure chart area with Y property
ChartArea chartArea = chart.ChartArea;
chartArea.Y = 20; // Setting Y position
chartArea.Height = 250;
workbook.Save("ChartAreaYExample.xlsx");
}
}
}
```
### See Also
* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
