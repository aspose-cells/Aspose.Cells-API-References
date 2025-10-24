##Axis.TickLabelSpacing
Axis property. Represents the number of categories or series between tickmark labels. Applies only to category and series axes
## Axis.TickLabelSpacing property
Represents the number of categories or series between tick-mark labels. Applies only to category and series axes.
```csharp
public int TickLabelSpacing { get; set; }
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
public class AxisPropertyTickLabelSpacingDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["A5"].PutValue("D");
worksheet.Cells["B5"].PutValue(40);
// Add chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data
chart.NSeries.Add("B2:B5", true);
chart.NSeries.CategoryData = "A2:A5";
// Configure axis tick label spacing
chart.CategoryAxis.TickLabelSpacing = 2; // Show every 2nd label
workbook.Save("AxisPropertyTickLabelSpacingDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
