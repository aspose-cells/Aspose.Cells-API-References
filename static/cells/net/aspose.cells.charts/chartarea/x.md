##ChartArea.X
ChartArea property. Gets or gets the horizontal offset from its upper left corner column in units of 1/4000 of the chart area
## ChartArea.X property
Gets or gets the horizontal offset from its upper left corner column, in units of 1/4000 of the chart area.
```csharp
[Obsolete("Use ChartArea.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Please use ChartArea.XRatioToChart property, instead. X = XRatioToChart * 4000. This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class ChartAreaPropertyXDemo
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
int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
// Configure chart area
Aspose.Cells.Charts.ChartArea chartArea = chart.ChartArea;
chartArea.X = 10; // Demonstrating X property usage
chartArea.Y = 10;
chartArea.Width = 400;
chartArea.Height = 300;
// Save output
workbook.Save("ChartAreaXDemo.xlsx");
}
}
}
```
### See Also
* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
