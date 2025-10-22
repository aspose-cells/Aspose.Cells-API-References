##Enum FormattingType
Aspose.Cells.Charts.FormattingType enum. Represents the type of formatting applied to an Area object or a Line object
## FormattingType enumeration
Represents the type of formatting applied to an [`Area`](../../aspose.cells.drawing/area/) object or a [`Line`](../../aspose.cells.drawing/line/) object.
```csharp
public enum FormattingType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Automatic | `0` | Represents automatic formatting type. |
| Custom | `2` | Represents custom formatting type. |
| None | `1` | Represents none formatting type. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
using System.Drawing;
public class FormattingTypeDemo
{
public static void FormattingTypeExample()
{
// Instantiate a Workbook object
Workbook workbook = new Workbook();
// Adding a new worksheet to the Workbook object
int sheetIndex = workbook.Worksheets.Add();
// Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[sheetIndex];
// Adding sample values to cells
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
// Adding a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
// Accessing the instance of the newly added chart
Chart chart = worksheet.Charts[chartIndex];
// Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", true);
// Setting the foreground color of the plot area
chart.PlotArea.Area.ForegroundColor = Color.Blue;
chart.PlotArea.Area.Formatting = FormattingType.Custom;
// Setting the foreground color of the chart area
chart.ChartArea.Area.ForegroundColor = Color.Yellow;
chart.ChartArea.Area.Formatting = FormattingType.Automatic;
// Setting the foreground color of the 1st NSeries area
chart.NSeries[0].Area.ForegroundColor = Color.Red;
chart.NSeries[0].Area.Formatting = FormattingType.None;
// Setting the foreground color of the area of the 1st NSeries point
chart.NSeries[0].Points[0].Area.ForegroundColor = Color.Cyan;
chart.NSeries[0].Points[0].Area.Formatting = FormattingType.Custom;
// Saving the Excel file
workbook.Save("FormattingTypeExample.xlsx");
workbook.Save("FormattingTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
