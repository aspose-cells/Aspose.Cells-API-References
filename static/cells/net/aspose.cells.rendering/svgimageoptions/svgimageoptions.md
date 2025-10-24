##SvgImageOptions.SvgImageOptions
SvgImageOptions constructor. Ctor
## SvgImageOptions constructor
Ctor.
```csharp
public SvgImageOptions()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;
using System;
public class SvgImageOptionsMethodCtorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Month");
worksheet.Cells["A2"].PutValue("Jan");
worksheet.Cells["A3"].PutValue("Feb");
worksheet.Cells["A4"].PutValue("Mar");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(120);
worksheet.Cells["B3"].PutValue(210);
worksheet.Cells["B4"].PutValue(150);
// Create a line chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B4", true);
chart.NSeries.CategoryData = "A2:A4";
try
{
// Create SvgImageOptions using the constructor
SvgImageOptions svgOptions = new SvgImageOptions();
// Configure SVG rendering options
svgOptions.ImageType = ImageType.Svg; // Explicitly set to SVG
svgOptions.FitToViewPort = true;
svgOptions.CssPrefix = "chart-prefix";
svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;
// Save the chart as SVG with specified options
chart.ToImage("output_chart.svg", svgOptions);
Console.WriteLine("SVG image saved successfully with specified options.");
}
catch (Exception ex)
{
Console.WriteLine($"Error generating SVG: {ex.Message}");
}
// Save the workbook to demonstrate the original data
workbook.Save("SvgImageOptionsDemo.xlsx");
}
}
}
```
### See Also
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
