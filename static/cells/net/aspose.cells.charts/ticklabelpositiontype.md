##Enum TickLabelPositionType
Aspose.Cells.Charts.TickLabelPositionType enum. Represents the position type of tickmark labels on the specified axis
## TickLabelPositionType enumeration
Represents the position type of tick-mark labels on the specified axis.
```csharp
public enum TickLabelPositionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| High | `0` | Position type is high. |
| Low | `1` | Position type is low. |
| NextToAxis | `2` | Position type is next to axis. |
| None | `3` | Position type is none. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class TickLabelPositionTypeDemo
{
public static void TickLabelPositionTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data to the worksheet
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(4);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(50);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", true);
// Access the category axis
Axis categoryAxis = chart.CategoryAxis;
// Set the tick label position to High
categoryAxis.TickLabelPosition = TickLabelPositionType.High;
// Save the workbook
workbook.Save("TickLabelPositionTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
