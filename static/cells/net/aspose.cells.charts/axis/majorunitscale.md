##Axis.MajorUnitScale
Axis property. Represents the major unit scale for the category axis
## Axis.MajorUnitScale property
Represents the major unit scale for the category axis.
```csharp
public TimeUnit MajorUnitScale { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyMajorUnitScaleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample time-scale data
worksheet.Cells["A1"].PutValue("Date");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue(new DateTime(2023, 3, 1));
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue(new DateTime(2023, 5, 1));
worksheet.Cells["B4"].PutValue(30);
// Create chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
// Configure category axis as time scale with major unit every 2 months
chart.CategoryAxis.CategoryType = CategoryType.TimeScale;
chart.CategoryAxis.MajorUnitScale = TimeUnit.Months;
chart.CategoryAxis.MajorUnit = 2;
workbook.Save("AxisPropertyMajorUnitScaleDemo_out.xlsx");
}
}
}
```
### See Also
* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
