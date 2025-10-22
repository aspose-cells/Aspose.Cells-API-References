##PlotArea.IsAutomaticSize
PlotArea property. Indicates whether the plot area is automatic sized
## PlotArea.IsAutomaticSize property
Indicates whether the plot area is automatic sized.
```csharp
public override bool IsAutomaticSize { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class PlotAreaPropertyIsAutomaticSizeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B4"].PutValue(30);
// Add chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Configure plot area
PlotArea plotArea = chart.PlotArea;
plotArea.IsAutomaticSize = false; // Disable automatic sizing
plotArea.Width = 3000;
plotArea.Height = 2000;
workbook.Save("PlotAreaIsAutomaticSizeDemo.xlsx");
}
}
}
```
### See Also
* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
