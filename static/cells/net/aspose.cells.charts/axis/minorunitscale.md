##Axis.MinorUnitScale
Axis property. Represents the major unit scale for the category axis
## Axis.MinorUnitScale property
Represents the major unit scale for the category axis.
```csharp
public TimeUnit MinorUnitScale { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyMinorUnitScaleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample time-based data
worksheet.Cells["A1"].PutValue("Date");
worksheet.Cells["B1"].PutValue("Value");
for (int i = 2; i <= 10; i++)
{
worksheet.Cells[$"A{i}"].PutValue(DateTime.Now.AddMonths(i - 2));
worksheet.Cells[$"B{i}"].PutValue(i * 100);
}
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data source
chart.NSeries.Add("B2:B10", true);
chart.NSeries.CategoryData = "A2:A10";
// Configure category axis as time scale
chart.CategoryAxis.CategoryType = CategoryType.TimeScale;
chart.CategoryAxis.MinorUnitScale = TimeUnit.Months;
chart.CategoryAxis.MinorUnit = 2;
// Save the workbook
workbook.Save("AxisPropertyMinorUnitScaleDemo.xlsx");
}
}
}
```
### See Also
* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
