##Series.Border
Series property. Represents border of Series object
## Series.Border property
Represents border of Series object.
```csharp
public Line Border { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class SeriesPropertyBorderDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Year");
worksheet.Cells["A2"].PutValue("2020");
worksheet.Cells["A3"].PutValue("2021");
worksheet.Cells["A4"].PutValue("2022");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(5000);
worksheet.Cells["B3"].PutValue(7000);
worksheet.Cells["B4"].PutValue(9000);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add series data
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Get the first series
Series series = chart.NSeries[0];
series.Name = "Sales Data";
// Customize the border properties
series.Border.Color = System.Drawing.Color.Blue;
series.Border.Weight = WeightType.MediumLine;
series.Border.DashType = MsoLineDashStyle.Solid;
series.Border.IsVisible = true;
// Save the workbook
workbook.Save("SeriesBorderDemo.xlsx");
}
}
}
```
### See Also
* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
