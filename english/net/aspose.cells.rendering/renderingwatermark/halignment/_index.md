---
title: RenderingWatermark.HAlignment
second_title: Aspose.Cells for .NET API Reference
description: RenderingWatermark property. Gets or sets horizontal alignment of the watermark to the page
type: docs
url: /net/aspose.cells.rendering/renderingwatermark/halignment/
---
## RenderingWatermark.HAlignment property

Gets or sets horizontal alignment of the watermark to the page.

```csharp
public TextAlignmentType HAlignment { get; set; }
```

### Remarks

Only Left, Center, Right is valid. Default is Left.

### Examples

```csharp
// Called: watermark.HAlignment = TextAlignmentType.Center;
public static void Property_HAlignment()
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

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


