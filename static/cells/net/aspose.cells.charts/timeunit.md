##Enum TimeUnit
Aspose.Cells.Charts.TimeUnit enum. Represents the base unit for the category axis
## TimeUnit enumeration
Represents the base unit for the category axis.
```csharp
public enum TimeUnit
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Days | `0` | Days |
| Months | `1` | Months |
| Years | `2` | Years |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class TimeUnitDemo
{
public static void TimeUnitExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1));
worksheet.Cells["A2"].PutValue(new DateTime(2023, 2, 1));
worksheet.Cells["A3"].PutValue(new DateTime(2023, 3, 1));
worksheet.Cells["B1"].PutValue(100);
worksheet.Cells["B2"].PutValue(200);
worksheet.Cells["B3"].PutValue(300);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 25, 10);
Chart chart = worksheet.Charts[chartIndex];
// Add series to the chart
chart.NSeries.Add("B1:B3", true);
chart.NSeries.CategoryData = "A1:A3";
// Set the category axis to use time units
Axis categoryAxis = chart.CategoryAxis;
categoryAxis.CategoryType = CategoryType.TimeScale;
categoryAxis.BaseUnitScale = TimeUnit.Months;
categoryAxis.MajorUnitScale = TimeUnit.Months;
categoryAxis.MinorUnitScale = TimeUnit.Days;
// Customize the appearance of the chart
chart.Title.Text = "Sample Chart with Time Units";
chart.ValueAxis.Title.Text = "Values";
chart.CategoryAxis.Title.Text = "Dates";
// Save the workbook
workbook.Save("TimeUnitExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
