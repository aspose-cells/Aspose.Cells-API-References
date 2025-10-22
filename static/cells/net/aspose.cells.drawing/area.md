##Class Area
Aspose.Cells.Drawing.Area class. Encapsulates the object that represents an area format
## Area class
Encapsulates the object that represents an area format.
```csharp
public class Area
```
## Properties
| Name | Description |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Gets or sets the background Color of the `Area`. |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Represents a [`FillFormat`](./fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Gets or sets the foreground Color. |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Represents the formatting of the area. |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class AreaDemo
{
public static void AreaExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Adding a new worksheet to the Workbook object
int sheetIndex = workbook.Worksheets.Add();
// Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.Worksheets[sheetIndex];
// Adding sample values to cells
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(-100);
worksheet.Cells["A3"].PutValue(150);
// Adding a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 15, 5);
// Accessing the instance of the newly added chart
Chart chart = worksheet.Charts[chartIndex];
// Adding NSeries (chart data source) to the chart ranging from "A1" cell to "A3"
chart.NSeries.Add("A1:A3", true);
// Accessing the area of the first NSeries
Area area = chart.NSeries[0].Area;
// Setting properties
area.InvertIfNegative = true;
area.ForegroundColor = Color.Red;
area.BackgroundColor = Color.Yellow;
area.Formatting = Aspose.Cells.Charts.FormattingType.Custom;
area.Transparency = 0.5;
// Saving the Excel file
workbook.Save("AreaExample.xlsx");
workbook.Save("AreaExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
