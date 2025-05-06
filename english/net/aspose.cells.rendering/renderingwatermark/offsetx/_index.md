---
title: RenderingWatermark.OffsetX
second_title: Aspose.Cells for .NET API Reference
description: RenderingWatermark property. Gets or sets offset value to HAlignment
type: docs
url: /net/aspose.cells.rendering/renderingwatermark/offsetx/
---
## RenderingWatermark.OffsetX property

Gets or sets offset value to [`HAlignment`](../halignment/)

```csharp
public float OffsetX { get; set; }
```

### Examples

```csharp
// Called: OffsetX = 0,
public static void Property_OffsetX()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            sheet.Cells[&quot;A1&quot;].PutValue(&quot;Hello World!&quot;);

            // Create a RenderingFont object
            RenderingFont renderingFont = new RenderingFont(&quot;Arial&quot;, 12)
            {
                Bold = true,
                Italic = true,
                Color = Color.Blue
            };

            // Create a RenderingWatermark object using the RenderingFont
            RenderingWatermark watermark = new RenderingWatermark(&quot;Sample Watermark&quot;, renderingFont)
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
            workbook.Save(&quot;RenderingFontExample.pdf&quot;, pdfSaveOptions);
        }
```

### See Also

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


