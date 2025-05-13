---
title: RenderingWatermark.OffsetY
second_title: Aspose.Cells for .NET API Reference
description: RenderingWatermark property. Gets or sets offset value to VAlignment
type: docs
url: /net/aspose.cells.rendering/renderingwatermark/offsety/
---
## RenderingWatermark.OffsetY property

Gets or sets offset value to [`VAlignment`](../valignment/)

```csharp
public float OffsetY { get; set; }
```

### Examples

```csharp
// Called: OffsetY = 0
public static void RenderingWatermark_Property_OffsetY()
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

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


