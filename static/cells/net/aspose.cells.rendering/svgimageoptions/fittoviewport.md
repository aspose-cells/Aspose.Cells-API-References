##SvgImageOptions.FitToViewPort
SvgImageOptions property. if this property is true the generated svg will fit to view port
## SvgImageOptions.FitToViewPort property
if this property is true, the generated svg will fit to view port.
```csharp
public bool FitToViewPort { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Rendering;
using System;
public class SvgImageOptionsPropertyFitToViewPortDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate cells with sample data
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["B1"].Value = "Quantity";
worksheet.Cells["B2"].Value = 150;
worksheet.Cells["B3"].Value = 250;
// Create a column chart
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 18, 6);
Chart chart = worksheet.Charts[chartIndex];
chart.NSeries.Add("B2:B3", true);
chart.NSeries.CategoryData = "A2:A3";
chart.Title.Text = "Sales Report";
// Create SVG rendering options
SvgImageOptions svgOptions = new SvgImageOptions();
// Display initial FitToViewPort value
Console.WriteLine($"Initial FitToViewPort: {svgOptions.FitToViewPort}");
// Modify the property and demonstrate effect
svgOptions.FitToViewPort = true;
Console.WriteLine($"Modified FitToViewPort: {svgOptions.FitToViewPort}");
// Render worksheet to SVG with different settings
SheetRender renderer = new SheetRender(worksheet, svgOptions);
renderer.ToImage(0, "FitToViewPortEnabled.svg");
// Optional: Create comparison with disabled FitToViewPort
svgOptions.FitToViewPort = false;
renderer = new SheetRender(worksheet, svgOptions);
renderer.ToImage(0, "FitToViewPortDisabled.svg");
Console.WriteLine("Generated SVG files demonstrate FitToViewPort effect.");
}
}
}
```
### See Also
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
