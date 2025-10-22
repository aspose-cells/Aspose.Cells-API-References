##Enum GradientDirectionType
Aspose.Cells.Drawing.GradientDirectionType enum. Represents all direction type of gradient
## GradientDirectionType enumeration
Represents all direction type of gradient.
```csharp
public enum GradientDirectionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| FromUpperLeftCorner | `0` | FromUpperLeftCorner |
| FromUpperRightCorner | `1` | FromUpperRightCorner |
| FromLowerLeftCorner | `2` | FromLowerLeftCorner |
| FromLowerRightCorner | `3` | FromLowerRightCorner |
| FromCenter | `4` | FromCenter |
| Unknown | `5` | Unknown |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class GradientDirectionTypeDemo
{
public static void GradientDirectionTypeExample()
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
// Set a two-color gradient fill with a specific direction
fillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.DiagonalDown, 1);
fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);
// Output the gradient direction type
Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);
// Save the workbook
workbook.Save("GradientDirectionTypeExample.xlsx");
workbook.Save("GradientDirectionTypeExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
