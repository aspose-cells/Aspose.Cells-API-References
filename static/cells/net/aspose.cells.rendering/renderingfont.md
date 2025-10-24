##Class RenderingFont
Aspose.Cells.Rendering.RenderingFont class. Font for rendering
## RenderingFont class
Font for rendering.
```csharp
public class RenderingFont
```
## Constructors
| Name | Description |
| --- | --- |
| [RenderingFont](renderingfont/)(string, float) | Initializes a new instance of the `RenderingFont` |
## Properties
| Name | Description |
| --- | --- |
| [Bold](../../aspose.cells.rendering/renderingfont/bold/) { get; set; } | Gets or sets bold for the font. |
| [Color](../../aspose.cells.rendering/renderingfont/color/) { get; set; } | Gets or sets color for the font. |
| [Italic](../../aspose.cells.rendering/renderingfont/italic/) { get; set; } | Gets or sets italic for the font. |
| [Name](../../aspose.cells.rendering/renderingfont/name/) { get; } | Gets name of the font. |
| [Size](../../aspose.cells.rendering/renderingfont/size/) { get; } | Gets size of the font in points. |
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
using System.Drawing;
namespace AsposeCellsExamples
{
public class RenderingFontDemo
{
public static void RenderingFontExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add some sample data
sheet.Cells["A1"].PutValue("Hello World!");
// Create a RenderingFont object
RenderingFont renderingFont = new RenderingFont("Arial", 12)
{
Bold = true,
Italic = true,
Color = Color.Blue
};
// Create a RenderingWatermark object using the RenderingFont
RenderingWatermark watermark = new RenderingWatermark("Sample Watermark", renderingFont)
{
Rotation = 45,
ScaleToPagePercent = 100,
Opacity = 0.5f,
IsBackground = true,
HAlignment = TextAlignmentType.Center,
VAlignment = TextAlignmentType.Center,
OffsetX = 0,
OffsetY = 0
};
// Create PdfSaveOptions and set the watermark
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions
{
Watermark = watermark,
EmbedStandardWindowsFonts = true,
CalculateFormula = true,
ExportDocumentStructure = true,
DisplayDocTitle = true
};
// Save the workbook to PDF with the watermark
workbook.Save("RenderingFontExample.pdf", pdfSaveOptions);
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
