##Enum ChartTextDirectionType
Aspose.Cells.Charts.ChartTextDirectionType enum. Represents the text direction type of the chart
## ChartTextDirectionType enumeration
Represents the text direction type of the chart.
```csharp
public enum ChartTextDirectionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Horizontal | `0` | Horizontal direction type. |
| Vertical | `1` | Vertical direction type. |
| Rotate90 | `2` | Rotate 90 angle. |
| Rotate270 | `3` | Rotate 270 angle. |
| Stacked | `4` | Stacked text. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
using System.Drawing;
public class ChartTextDirectionTypeDemo
{
public static void ChartTextDirectionTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add data series to the chart
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Set the title of the chart
chart.Title.Text = "Sample Chart";
chart.Title.Font.Color = Color.Blue;
// Set the text direction of the chart title
chart.Title.DirectionType = ChartTextDirectionType.Rotate90;
// Set the text direction of the category axis title
chart.CategoryAxis.Title.Text = "Categories";
chart.CategoryAxis.Title.DirectionType = ChartTextDirectionType.Vertical;
// Set the text direction of the value axis title
chart.ValueAxis.Title.Text = "Values";
chart.ValueAxis.Title.DirectionType = ChartTextDirectionType.Horizontal;
// Save the workbook
workbook.Save("ChartTextDirectionTypeExample.xlsx");
workbook.Save("ChartTextDirectionTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
