##Class LegendEntry
Aspose.Cells.Charts.LegendEntry class. Represents a legend entry in a chart legend
## LegendEntry class
Represents a legend entry in a chart legend.
```csharp
public class LegendEntry
```
## Properties
| Name | Description |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/legendentry/autoscalefont/) { get; set; } | True if the text in the object changes font size when the object size changes. The default value is True. |
| [Background](../../aspose.cells.charts/legendentry/background/) { get; set; } | (**Obsolete.**) Gets and sets the display mode of the background |
| [BackgroundMode](../../aspose.cells.charts/legendentry/backgroundmode/) { get; set; } | Gets and sets the display mode of the background |
| [Font](../../aspose.cells.charts/legendentry/font/) { get; } | Gets a [`Font`](./font/) object of the specified ChartFrame object. |
| [IsDeleted](../../aspose.cells.charts/legendentry/isdeleted/) { get; set; } | Gets and sets whether the legend entry is deleted. |
| [IsTextNoFill](../../aspose.cells.charts/legendentry/istextnofill/) { get; set; } | Gets or sets no fill of the text. |
| virtual [TextFont](../../aspose.cells.charts/legendentry/textfont/) { get; } | (**Obsolete.**) Gets a [`Font`](./font/) object of the specified LegendEntry object. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
public class LegendEntryDemo
{
public static void LegendEntryExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["A4"].PutValue(200);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
worksheet.Cells["B4"].PutValue(40);
worksheet.Cells["C1"].PutValue("Q1");
worksheet.Cells["C2"].PutValue("Q2");
worksheet.Cells["C3"].PutValue("Y1");
worksheet.Cells["C4"].PutValue("Y2");
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", true);
chart.NSeries.CategoryData = "C1:C4";
// Access the legend entry of the first series
LegendEntry legendEntry = chart.NSeries[0].LegendEntry;
// Set properties of the legend entry
legendEntry.IsDeleted = false;
legendEntry.IsTextNoFill = false;
legendEntry.AutoScaleFont = true;
legendEntry.Background = BackgroundMode.Transparent;
legendEntry.BackgroundMode = BackgroundMode.Opaque;
// Access and modify the font of the legend entry
Font font = legendEntry.Font;
font.Name = "Arial";
font.Size = 12;
font.IsBold = true;
font.Color = System.Drawing.Color.Blue;
// Save the workbook
workbook.Save("LegendEntryExample.xlsx");
workbook.Save("LegendEntryExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
