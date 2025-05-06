---
title: PdfSaveOptions.ExportDocumentStructure
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions property. Indicates whether to export document structure
type: docs
url: /net/aspose.cells/pdfsaveoptions/exportdocumentstructure/
---
## PdfSaveOptions.ExportDocumentStructure property

Indicates whether to export document structure.

```csharp
public bool ExportDocumentStructure { get; set; }
```

### Examples

```csharp
// Called: ExportDocumentStructure = true,
public static void Property_ExportDocumentStructure()
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

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


