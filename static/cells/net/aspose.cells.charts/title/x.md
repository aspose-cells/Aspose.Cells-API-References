##Title.X
Title property. Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area
## Title.X property
Gets or sets the x coordinate of the upper left corner in units of 1/4000 of the chart area.
```csharp
[Obsolete("Use Title.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Please use Title.XRatioToChart property, instead. X = XRatioToChart * 4000; This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class TitlePropertyXDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["A2"].PutValue("A");
sheet.Cells["A3"].PutValue("B");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["B3"].PutValue(20);
// Add chart and set data
int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
// Set chart title properties with X position
chart.Title.Text = "Sample Chart";
chart.Title.X = 200; // Demonstrating X property usage
chart.Title.Y = 50;
// Save the workbook
workbook.Save("TitlePropertyXDemo.xlsx");
}
}
}
```
### See Also
* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
