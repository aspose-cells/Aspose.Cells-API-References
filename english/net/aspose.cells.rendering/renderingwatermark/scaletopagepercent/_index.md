---
title: RenderingWatermark.ScaleToPagePercent
second_title: Aspose.Cells for .NET API Reference
description: RenderingWatermark property. Gets or sets scale relative to target page in percent
type: docs
url: /net/aspose.cells.rendering/renderingwatermark/scaletopagepercent/
---
## RenderingWatermark.ScaleToPagePercent property

Gets or sets scale relative to target page in percent.

```csharp
public int ScaleToPagePercent { get; set; }
```

### Examples

```csharp
// Called: watermark.ScaleToPagePercent = 50;
public static void Property_ScaleToPagePercent()
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
```

### See Also

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


