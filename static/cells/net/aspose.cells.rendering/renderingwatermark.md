##Class RenderingWatermark
Aspose.Cells.Rendering.RenderingWatermark class. Watermark for rendering
## RenderingWatermark class
Watermark for rendering.
```csharp
public class RenderingWatermark
```
## Constructors
| Name | Description |
| --- | --- |
| [RenderingWatermark](renderingwatermark/#constructor)(byte[]) | Creates instance of image watermark. |
| [RenderingWatermark](renderingwatermark/#constructor_1)(string, RenderingFont) | Creates instance of text watermark. |
## Properties
| Name | Description |
| --- | --- |
| [Font](../../aspose.cells.rendering/renderingwatermark/font/) { get; } | Gets font of the watermark. |
| [HAlignment](../../aspose.cells.rendering/renderingwatermark/halignment/) { get; set; } | Gets or sets horizontal alignment of the watermark to the page. |
| [Image](../../aspose.cells.rendering/renderingwatermark/image/) { get; } | Gets image of the watermark. |
| [IsBackground](../../aspose.cells.rendering/renderingwatermark/isbackground/) { get; set; } | Indicates whether the watermark is placed behind page contents. |
| [OffsetX](../../aspose.cells.rendering/renderingwatermark/offsetx/) { get; set; } | Gets or sets offset value to [`HAlignment`](./halignment/) |
| [OffsetY](../../aspose.cells.rendering/renderingwatermark/offsety/) { get; set; } | Gets or sets offset value to [`VAlignment`](./valignment/) |
| [Opacity](../../aspose.cells.rendering/renderingwatermark/opacity/) { get; set; } | Gets or sets opacity of the watermark in range [0, 1]. |
| [Rotation](../../aspose.cells.rendering/renderingwatermark/rotation/) { get; set; } | Gets or sets roation of the watermark in degrees. |
| [ScaleToPagePercent](../../aspose.cells.rendering/renderingwatermark/scaletopagepercent/) { get; set; } | Gets or sets scale relative to target page in percent. |
| [Text](../../aspose.cells.rendering/renderingwatermark/text/) { get; } | Gets text of the watermark. |
| [VAlignment](../../aspose.cells.rendering/renderingwatermark/valignment/) { get; set; } | Gets or sets vertical alignment of the watermark to the page. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
using System.Drawing;
public class RenderingWatermarkDemo
{
public static void RenderingWatermarkExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("This is a sample worksheet.");
// Create a font for the watermark
RenderingFont font = new RenderingFont("Calibri", 68);
font.Italic = true;
font.Bold = true;
font.Color = Color.Blue;
// Create a watermark from text and the specified font
RenderingWatermark watermark = new RenderingWatermark("Watermark", font);
// Set properties for the watermark
watermark.HAlignment = TextAlignmentType.Center;
watermark.VAlignment = TextAlignmentType.Center;
watermark.Rotation = 30;
watermark.Opacity = 0.6f;
watermark.ScaleToPagePercent = 50;
watermark.IsBackground = true;
// Specify watermark for rendering to PDF
PdfSaveOptions options = new PdfSaveOptions();
options.Watermark = watermark;
// Save the workbook as a PDF with the watermark
workbook.Save("output_watermark.pdf", options);
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
