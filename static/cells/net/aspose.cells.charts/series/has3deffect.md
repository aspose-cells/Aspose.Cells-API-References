##Series.Has3DEffect
Series property. True if the series has a threedimensional appearance. Applies only to bubble charts
## Series.Has3DEffect property
True if the series has a three-dimensional appearance. Applies only to bubble charts.
```csharp
public bool Has3DEffect { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class SeriesPropertyHas3DEffectDemo
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
worksheet.Cells["C1"].PutValue("Q1");
worksheet.Cells["C2"].PutValue("Q2");
worksheet.Cells["C3"].PutValue("Q3");
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add series
int seriesIndex = chart.NSeries.Add("A1:B3", true);
chart.NSeries.CategoryData = "C1:C3";
// Get the series and set 3D effect
Series series = chart.NSeries[seriesIndex];
series.Has3DEffect = true;
series.Bar3DShapeType = Bar3DShapeType.Cylinder;
// Save the workbook
workbook.Save("Series3DEffectDemo.xlsx");
}
}
}
```
### See Also
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
