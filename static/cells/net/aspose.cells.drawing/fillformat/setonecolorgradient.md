##FillFormat.SetOneColorGradient
FillFormat method. Sets the specified fill to a onecolor gradient. Only applies for Excel 2007
## FillFormat.SetOneColorGradient method
Sets the specified fill to a one-color gradient. Only applies for Excel 2007.
```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```
| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | One gradient color. |
| degree | Double | The gradient degree. Can be a value from 0.0 (dark) through 1.0 (light). |
| style | GradientStyleType | Gradient shading style. |
| variant | Int32 | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class FillFormatMethodSetOneColorGradientWithColorDoubleGradientStyleTypeInDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for chart
worksheet.Cells["A1"].PutValue("Series 1");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["A4"].PutValue(3);
worksheet.Cells["B1"].PutValue("Values");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
// Set chart data range
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
// Apply gradient fill to the first series
Series series = chart.NSeries[0];
series.IsColorVaried = false;
// Demonstrate SetOneColorGradient with specific parameters
series.Area.FillFormat.SetOneColorGradient(
Color.FromArgb(0, 236, 102, 102), // Color
0.9,                              // Transparency
Aspose.Cells.Drawing.GradientStyleType.DiagonalDown,    // Gradient style
2);                                // Variant
// Save the workbook
workbook.Save("FillFormat_SetOneColorGradient_Output.xlsx");
}
}
}
```
### See Also
* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
