##SvgImageOptions.EmbeddedFontType
SvgImageOptions property. Gets or sets the type of font that embedded in Svg
## SvgImageOptions.EmbeddedFontType property
Gets or sets the type of font that embedded in Svg.
```csharp
public SvgEmbeddedFontType EmbeddedFontType { get; set; }
```
### Remarks
Default value is None which indicates that it will not embed font in Svg.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class SvgImageOptionsPropertyEmbeddedFontTypeDemo
{
public static void Run()
{
// Create a new workbook and access the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add data with custom formatting to demonstrate font embedding
var cell = worksheet.Cells["B2"];
cell.PutValue("SVG Font Embedding Test");
Style style = workbook.CreateStyle();
style.Font.Name = "Arial";
style.Font.Size = 14;
cell.SetStyle(style);
// Create SVG rendering options
SvgImageOptions svgOptions = new SvgImageOptions();
// Display initial embedded font type
Console.WriteLine($"Initial EmbeddedFontType: {svgOptions.EmbeddedFontType}");
// Render worksheet to SVG without font embedding
SheetRender renderer = new SheetRender(worksheet, svgOptions);
renderer.ToImage(0, "WithoutFontEmbedding.svg");
// Change embedded font type to WOFF
svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;
// Render worksheet to SVG with WOFF font embedding
SheetRender renderer2 = new SheetRender(worksheet, svgOptions);
renderer2.ToImage(0, "WithWoffFontEmbedding.svg");
Console.WriteLine("Generated SVG files with different font embedding settings.");
}
}
}
```
### See Also
* enum [SvgEmbeddedFontType](../../svgembeddedfonttype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
