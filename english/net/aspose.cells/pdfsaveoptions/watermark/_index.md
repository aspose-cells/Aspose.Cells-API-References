---
title: PdfSaveOptions.Watermark
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions property. Gets or sets watermark to output
type: docs
url: /net/aspose.cells/pdfsaveoptions/watermark/
---
## PdfSaveOptions.Watermark property

Gets or sets watermark to output.

```csharp
public RenderingWatermark Watermark { get; set; }
```

### Examples

The following code sets watermark in the output pdf.

```csharp
//prepare a workbook with 3 pages.
Workbook wb = new Workbook();
wb.Worksheets[0].Cells["A1"].PutValue("Page1");
int index = wb.Worksheets.Add();
wb.Worksheets[index].Cells["A1"].PutValue("Page2");
index = wb.Worksheets.Add();
wb.Worksheets[index].Cells["A1"].PutValue("Page3");
wb.Worksheets[index].PageSetup.PaperSize = PaperSizeType.PaperA3;

//create a font for watermark, and specify bold, italic, color
RenderingFont font = new RenderingFont("Calibri", 68);
font.Italic = true;
font.Bold = true;
font.Color = Color.Blue;

//create a watermark from text and the specified font
RenderingWatermark watermark = new RenderingWatermark("Watermark", font);

//specify horizontal and vertical alignment
watermark.HAlignment = TextAlignmentType.Center;
watermark.VAlignment = TextAlignmentType.Center;

//specify rotation
watermark.Rotation = 30;

//specify opacity
watermark.Opacity = 0.6f;

//specify the scale to page(e.g. 100, 50) in percent.
watermark.ScaleToPagePercent = 50;

//spcify watermark for rendering to pdf.
PdfSaveOptions options = new PdfSaveOptions();
options.Watermark = watermark;

wb.Save("output_watermark.pdf", options);
```

### See Also

* class [RenderingWatermark](../../../aspose.cells.rendering/renderingwatermark/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


