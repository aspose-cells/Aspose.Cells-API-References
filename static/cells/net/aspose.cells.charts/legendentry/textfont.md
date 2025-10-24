##LegendEntry.TextFont
LegendEntry property. Gets a Font object of the specified LegendEntry object
## LegendEntry.TextFont property
Gets a [`Font`](../font/) object of the specified LegendEntry object.
```csharp
[Obsolete("Use LegendEntry.Font property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual Font TextFont { get; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use LegendEntry.Font property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class LegendEntryPropertyTextFontDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Series 1");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(20);
worksheet.Cells["A4"].PutValue(30);
worksheet.Cells["B1"].PutValue("Series 2");
worksheet.Cells["B2"].PutValue(25);
worksheet.Cells["B3"].PutValue(35);
worksheet.Cells["B4"].PutValue(45);
// Add a chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("A2:A4", true);
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A1:B1";
// Enable legend
chart.ShowLegend = true;
Legend legend = chart.Legend;
// Access first legend entry and modify its TextFont properties
LegendEntry legendEntry = legend.LegendEntries[0];
Aspose.Cells.Font font = legendEntry.TextFont;
// Set various font properties
font.Name = "Arial";
font.Size = 12;
font.Color = Color.Red;
font.IsBold = true;
font.IsItalic = true;
font.Underline = FontUnderlineType.Single;
// Save the workbook
workbook.Save("LegendEntryTextFontDemo.xlsx");
}
}
}
```
### See Also
* class [Font](../../../aspose.cells/font/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)
