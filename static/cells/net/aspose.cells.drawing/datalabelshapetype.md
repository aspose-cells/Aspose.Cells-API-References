##Enum DataLabelShapeType
Aspose.Cells.Drawing.DataLabelShapeType enum. Specifies the preset shape geometry that is to be used for a chart
## DataLabelShapeType enumeration
Specifies the preset shape geometry that is to be used for a chart.
```csharp
public enum DataLabelShapeType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Rect | `0` | Represents the rectangle shape. |
| RoundRect | `1` | Represents the round rectangle shape. |
| Ellipse | `2` | Represents the ellipse shape. |
| RightArrowCallout | `3` | Represents the right arrow callout shape. |
| DownArrowCallout | `4` | Represents the down arrow callout shape. |
| LeftArrowCallout | `5` | Represents the left arrow callout shape. |
| UpArrowCallout | `6` | Represents the up arrow callout shape. |
| WedgeRectCallout | `7` | Represents the wedge rectangle callout shape. |
| WedgeRoundRectCallout | `8` | Represents the wedge round rectangle callout shape. |
| WedgeEllipseCallout | `9` | Represents the wedge ellipse callout shape. |
| LineCallout | `10` | Represents the line callout shape. |
| BentLineCallout | `11` | Represents the bent line callout shape. |
| LineWithAccentBarCallout | `12` | Represents the line with accent bar callout shape. |
| BentLineWithAccentBarCallout | `13` | Represents the bent line with accent bar callout shape. |
| Line | `14` | This type is only used for special file processing |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
public class DataLabelShapeTypeDemo
{
public static void DataLabelShapeTypeExample()
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
// Set the chart data range
chart.SetChartDataRange("A1:B4", true);
// Access the first series in the chart
Series series = chart.NSeries[0];
// Enable data labels for the series
series.DataLabels.ShowValue = true;
series.DataLabels.ShapeType = DataLabelShapeType.RoundRect;
// Save the workbook
workbook.Save("DataLabelShapeTypeExample.xlsx");
workbook.Save("DataLabelShapeTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
