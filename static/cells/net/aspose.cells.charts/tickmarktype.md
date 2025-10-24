##Enum TickMarkType
Aspose.Cells.Charts.TickMarkType enum. Represents the tick mark type for the specified axis
## TickMarkType enumeration
Represents the tick mark type for the specified axis.
```csharp
public enum TickMarkType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Cross | `0` | Tick mark type is Cross. |
| Inside | `1` | Tick mark type is Inside. |
| None | `2` | Tick mark type is None. |
| Outside | `3` | Tick mark type is Outside |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class TickMarkTypeDemo
{
public static void TickMarkTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
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
// Access the value axis of the chart
Axis valueAxis = chart.ValueAxis;
// Set the major tick mark type to Cross
valueAxis.MajorTickMark = TickMarkType.Cross;
// Set the minor tick mark type to Inside
valueAxis.MinorTickMark = TickMarkType.Inside;
// Set the max value of value axis
valueAxis.MaxValue = 200;
// Set the min value of value axis
valueAxis.MinValue = 0;
// Set the major unit
valueAxis.MajorUnit = 25;
// Save the workbook
workbook.Save("TickMarkTypeExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
