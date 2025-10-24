##Axis.AxisBetweenCategories
Axis property. Represents if the value axis crosses the category axis between categories
## Axis.AxisBetweenCategories property
Represents if the value axis crosses the category axis between categories.
```csharp
public bool AxisBetweenCategories { get; set; }
```
### Remarks
This property applies only to category axes, and it doesn't apply to 3-D charts.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;
namespace AsposeCellsExamples
{
public class AxisPropertyAxisBetweenCategoriesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet and add sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Categories");
worksheet.Cells["B1"].PutValue("Values");
for (int i = 1; i <= 5; i++)
{
worksheet.Cells[$"A{i+1}"].PutValue($"Category {i}");
worksheet.Cells[$"B{i+1}"].PutValue(i * 10);
}
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data
chart.NSeries.Add("B2:B6", true);
chart.NSeries.CategoryData = "A2:A6";
// Configure category axis
Axis categoryAxis = chart.CategoryAxis;
categoryAxis.AxisBetweenCategories = false; // Core property demonstration
categoryAxis.TickLabels.RotationAngle = 45;
// Save the workbook
workbook.Save("AxisBetweenCategoriesDemo.xlsx");
}
}
}
```
### See Also
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
