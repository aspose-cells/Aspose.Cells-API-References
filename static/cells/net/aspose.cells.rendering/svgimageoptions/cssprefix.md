##SvgImageOptions.CssPrefix
SvgImageOptions property. Gets and sets the prefix of the css name in svgthe default value is empty string
## SvgImageOptions.CssPrefix property
Gets and sets the prefix of the css name in svg,the default value is empty string.
```csharp
public string CssPrefix { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Rendering;
using System;
using System.IO;
public class SvgImageOptionsPropertyCssPrefixDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the chart
worksheet.Cells["A1"].PutValue("Year");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue(2019);
worksheet.Cells["A3"].PutValue(2020);
worksheet.Cells["A4"].PutValue(2021);
worksheet.Cells["A5"].PutValue(2022);
worksheet.Cells["B2"].PutValue(4500);
worksheet.Cells["B3"].PutValue(4900);
worksheet.Cells["B4"].PutValue(5200);
worksheet.Cells["B5"].PutValue(6100);
// Create a line chart
int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
Chart chart = worksheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B5", true);
// Create SVG image options
SvgImageOptions svgOptions = new SvgImageOptions();
// Display current CSS prefix
Console.WriteLine("Current CssPrefix value: " + svgOptions.CssPrefix);
// Set new CSS prefix
svgOptions.CssPrefix = "chart-prefix-";
// Demonstrate SVG generation with custom CSS prefix
string outputPath = "output_chart.svg";
chart.ToImage(outputPath, svgOptions);
Console.WriteLine("Chart saved as SVG with custom CSS prefix.");
}
}
}
```
### See Also
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
