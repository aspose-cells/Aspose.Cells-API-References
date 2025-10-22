##Enum CrossType
Aspose.Cells.Charts.CrossType enum. Represents the axis cross type
## CrossType enumeration
Represents the axis cross type.
```csharp
public enum CrossType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Automatic | `0` | Microsoft Excel sets the axis crossing point. |
| Maximum | `1` | The axis crosses at the maximum value. |
| Minimum | `2` | The axis crosses at the minimum value. |
| Custom | `3` | The axis crosses at the custom value. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class CrossTypeDemo
{
public static void CrossTypeExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Adding a new worksheet to the Excel object
int sheetIndex = workbook.Worksheets.Add();
// Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[sheetIndex];
// Adding sample values to cells
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(4);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(50);
// Adding a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
// Accessing the instance of the newly added chart
Chart chart = worksheet.Charts[chartIndex];
// Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", true);
// Set the max value of value axis
chart.ValueAxis.MaxValue = 200;
// Set the min value of value axis
chart.ValueAxis.MinValue = 0;
// Set the major unit
chart.ValueAxis.MajorUnit = 25;
// Category(X) axis crosses at the maximum value
chart.ValueAxis.CrossType = CrossType.Maximum;
// Set the number of categories or series between tick-mark labels
chart.CategoryAxis.TickLabelSpacing = 2;
// Saving the Excel file
workbook.Save("CrossTypeExample.xlsx");
workbook.Save("CrossTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
