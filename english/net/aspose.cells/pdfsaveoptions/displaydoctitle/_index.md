---
title: PdfSaveOptions.DisplayDocTitle
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions property. Indicates whether the windows title bar should display the document title
type: docs
url: /net/aspose.cells/pdfsaveoptions/displaydoctitle/
---
## PdfSaveOptions.DisplayDocTitle property

Indicates whether the window's title bar should display the document title.

```csharp
public bool DisplayDocTitle { get; set; }
```

### Remarks

If false, the title bar should instead display the name of the PDF file. Default value is false.

### Examples

```csharp
// Called: DisplayDocTitle = true
public static void Property_DisplayDocTitle()
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


