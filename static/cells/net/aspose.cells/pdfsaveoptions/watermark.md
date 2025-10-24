##PdfSaveOptions.Watermark
PdfSaveOptions property. Gets or sets watermark to output
## PdfSaveOptions.Watermark property
Gets or sets watermark to output.
```csharp
public RenderingWatermark Watermark { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class PdfSaveOptionsPropertyWatermarkDemo
{
public static void Run()
{
// Create a workbook with 3 worksheets
Workbook wb = new Workbook();
wb.Worksheets[0].Cells["A1"].PutValue("Page1");
int index = wb.Worksheets.Add();
wb.Worksheets[index].Cells["A1"].PutValue("Page2");
index = wb.Worksheets.Add();
wb.Worksheets[index].Cells["A1"].PutValue("Page3");
// Create watermark font
RenderingFont font = new RenderingFont("Calibri", 68);
font.Italic = true;
font.Bold = true;
font.Color = Color.Blue;
// Create watermark with text and font
RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
watermark.HAlignment = TextAlignmentType.Center;
watermark.VAlignment = TextAlignmentType.Center;
watermark.Rotation = 45;
watermark.Opacity = 0.3f;
watermark.ScaleToPagePercent = 75;
// Set watermark in PDF save options
PdfSaveOptions options = new PdfSaveOptions();
options.Watermark = watermark;
// Save workbook with watermark
wb.Save("output_watermark.pdf", options);
}
}
}
```
### See Also
* class [RenderingWatermark](../../../aspose.cells.rendering/renderingwatermark/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
