##Axis.TickMarkSpacing
Axis property. Returns or sets the number of categories or series between tick marks. Applies only to category and series axes
## Axis.TickMarkSpacing property
Returns or sets the number of categories or series between tick marks. Applies only to category and series axes.
```csharp
public int TickMarkSpacing { get; set; }
```
### Remarks
The number must be between 1 and 31999.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyTickMarkSpacingDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(4);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(50);
// Add chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("A1:B3", true);
// Configure value axis with TickMarkSpacing
Axis valueAxis = chart.ValueAxis;
valueAxis.MinValue = 0;
valueAxis.MaxValue = 200;
valueAxis.MajorUnit = 25;
valueAxis.MinorUnit = 5;
valueAxis.TickMarkSpacing = 2; // Setting tick mark spacing
// Configure category axis with TickMarkSpacing
Axis categoryAxis = chart.CategoryAxis;
categoryAxis.TickMarkSpacing = 1; // Setting tick mark spacing
workbook.Save("AxisTickMarkSpacingDemo.xlsx");
}
}
}
```
### See Also
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
