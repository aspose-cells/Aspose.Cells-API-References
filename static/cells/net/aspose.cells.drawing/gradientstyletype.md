##Enum GradientStyleType
Aspose.Cells.Drawing.GradientStyleType enum. Represents gradient shading style
## GradientStyleType enumeration
Represents gradient shading style.
```csharp
public enum GradientStyleType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| DiagonalDown | `0` | Diagonal down shading style |
| DiagonalUp | `1` | Diagonal up shading style |
| FromCenter | `2` | From center shading style |
| FromCorner | `3` | From corner shading style |
| Horizontal | `4` | Horizontal shading style |
| Vertical | `5` | Vertical shading style |
| Unknown | `6` | Unknown shading style.Only for the shading style(which is not for any member of the GradientStyleType) in the template file. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class GradientStyleTypeDemo
{
public static void GradientStyleTypeExample()
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
// Access the chart's plot area
PlotArea plotArea = chart.PlotArea;
// Access the fill format of the plot area
FillFormat fillFormat = plotArea.Area.FillFormat;
// Set a two-color gradient fill with DiagonalDown style
fillFormat.SetTwoColorGradient(Color.Blue, Color.White, GradientStyleType.DiagonalDown, 1);
// Output the gradient style used
Console.WriteLine("Gradient Style: " + fillFormat.GradientStyle);
// Save the workbook
workbook.Save("GradientStyleTypeExample.xlsx");
workbook.Save("GradientStyleTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
