---
title: RenderingFont.RenderingFont
second_title: Aspose.Cells for .NET API Reference
description: RenderingFont constructor. Initializes a new instance of the RenderingFont
type: docs
url: /net/aspose.cells.rendering/renderingfont/renderingfont/
---
## RenderingFont constructor

Initializes a new instance of the [`RenderingFont`](../)

```csharp
public RenderingFont(string fontName, float fontSize)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fontName | String | font name |
| fontSize | Single | font size in points |

### Examples

```csharp
// Called: RenderingFont font = new RenderingFont(&amp;quot;Calibri&amp;quot;, 68);
public static void RenderingFont_Constructor()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;This is a sample worksheet.&quot;);

            // Create a font for the watermark
            RenderingFont font = new RenderingFont(&quot;Calibri&quot;, 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // Create a watermark from text and the specified font
            RenderingWatermark watermark = new RenderingWatermark(&quot;Watermark&quot;, font);

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
            workbook.Save(&quot;output_watermark.pdf&quot;, options);
        }
```

### See Also

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


