##Axis.BaseUnitScale
Axis property. Represents the base unit scale for the category axis
## Axis.BaseUnitScale property
Represents the base unit scale for the category axis.
```csharp
public TimeUnit BaseUnitScale { get; set; }
```
### Remarks
Setting this property only takes effect when the CategoryType property is set to TimeScale.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyBaseUnitScaleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for the chart
sheet.Cells["A1"].PutValue("Date");
sheet.Cells["B1"].PutValue("Value");
for (int i = 2; i <= 10; i++)
{
sheet.Cells[$"A{i}"].PutValue(DateTime.Now.AddDays(i));
sheet.Cells[$"B{i}"].PutValue(i * 100);
}
// Add a chart
int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
Chart chart = sheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B10", true);
chart.NSeries.CategoryData = "A2:A10";
// Set base unit scale for category axis
chart.CategoryAxis.BaseUnitScale = TimeUnit.Months;
// Save the workbook
workbook.Save("AxisPropertyBaseUnitScaleDemo_out.xlsx");
}
}
}
```
### See Also
* enum [TimeUnit](../../timeunit/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
