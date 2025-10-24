##Enum SvgEmbeddedFontType
Aspose.Cells.Rendering.SvgEmbeddedFontType enum. Represents the embedded font type in Svg image
## SvgEmbeddedFontType enumeration
Represents the embedded font type in Svg image.
```csharp
public enum SvgEmbeddedFontType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Not Embed font. |
| Woff | `1` | Embed WOFF font. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Rendering;
using System;
public class RenderingClassSvgEmbeddedFontTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue(50);
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(150);
worksheet.Cells["B1"].PutValue(4);
worksheet.Cells["B2"].PutValue(20);
worksheet.Cells["B3"].PutValue(50);
// Add a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B1:B3", true);
chart.NSeries.CategoryData = "A1:A3";
// Configure SVG image options
SvgImageOptions svgOptions = new SvgImageOptions
{
EmbeddedFontType = SvgEmbeddedFontType.Woff,
FitToViewPort = true,
CssPrefix = "chart-prefix"
};
// Save the chart as SVG with embedded WOFF font
chart.ToImage("output_chart.svg", svgOptions);
Console.WriteLine("SVG with embedded WOFF font generated successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
