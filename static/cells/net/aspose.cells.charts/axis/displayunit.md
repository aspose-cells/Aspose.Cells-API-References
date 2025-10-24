##Axis.DisplayUnit
Axis property. Represents the unit label for the specified axis
## Axis.DisplayUnit property
Represents the unit label for the specified axis.
```csharp
public DisplayUnitType DisplayUnit { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class AxisPropertyDisplayUnitDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10000);
worksheet.Cells["B3"].PutValue(20000);
worksheet.Cells["B4"].PutValue(30000);
// Add a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Set display unit for value axis to thousands
chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
// Save the workbook
workbook.Save("AxisPropertyDisplayUnitDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* enum [DisplayUnitType](../../displayunittype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
