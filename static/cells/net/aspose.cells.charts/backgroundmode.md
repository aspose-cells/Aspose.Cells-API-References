##Enum BackgroundMode
Aspose.Cells.Charts.BackgroundMode enum. Represents the display mode of the background
## BackgroundMode enumeration
Represents the display mode of the background.
```csharp
public enum BackgroundMode
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Automatic | `0` | Automatic |
| Opaque | `1` | Opaque |
| Transparent | `2` | Transparent |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using System;
using System.Drawing;
public class BackgroundModeDemo
{
public static void BackgroundModeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Obtain the reference of the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data to cells
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(60);
worksheet.Cells["B2"].PutValue(32);
worksheet.Cells["B3"].PutValue(50);
// Add a chart to the worksheet
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
// Add NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", true);
// Access the chart area
ChartArea chartArea = chart.ChartArea;
// Set the foreground color of the chart area
chartArea.Area.ForegroundColor = Color.Yellow;
// Set the background mode of the chart area
chartArea.BackgroundMode = BackgroundMode.Opaque;
chartArea.Area.Transparency = 0.8;
// Set the shadow of the chart area
chartArea.Shadow = true;
// Save the workbook
workbook.Save("BackgroundModeExample.xlsx");
workbook.Save("BackgroundModeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)
