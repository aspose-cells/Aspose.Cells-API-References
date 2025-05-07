---
title: RenderingWatermark.RenderingWatermark
second_title: Aspose.Cells for .NET API Reference
description: RenderingWatermark constructor. Creates instance of text watermark
type: docs
url: /net/aspose.cells.rendering/renderingwatermark/renderingwatermark/
---
## RenderingWatermark(string, RenderingFont) {#constructor_1}

Creates instance of text watermark.

```csharp
public RenderingWatermark(string text, RenderingFont renderingFont)
```

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | watermark text |
| renderingFont | RenderingFont | watermark font |

### Examples

```csharp
// Called: RenderingWatermark watermark = new RenderingWatermark("Sample Watermark", renderingFont)
public static void RenderingWatermark_Constructor()
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
```

### See Also

* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## RenderingWatermark(byte[]) {#constructor}

Creates instance of image watermark.

```csharp
public RenderingWatermark(byte[] imageData)
```

| Parameter | Type | Description |
| --- | --- | --- |
| imageData | Byte[] |  |

### See Also

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


