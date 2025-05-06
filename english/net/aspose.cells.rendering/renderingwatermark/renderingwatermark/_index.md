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
// Called: RenderingWatermark watermark = new RenderingWatermark(&amp;quot;Watermark&amp;quot;, font)
public static void RenderingWatermark_Constructor()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Aspose.Cells PDF Save Options Example&quot;);

            // Create an instance of PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Set various properties
            pdfSaveOptions.EmbedStandardWindowsFonts = true;
            pdfSaveOptions.Compliance = PdfCompliance.PdfA1b;
            pdfSaveOptions.CalculateFormula = true;
            pdfSaveOptions.PdfCompression = PdfCompressionCore.Flate;
            pdfSaveOptions.CreatedTime = DateTime.Now;
            pdfSaveOptions.Producer = &quot;Aspose.Cells&quot;;
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;
            pdfSaveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;
            pdfSaveOptions.ExportDocumentStructure = true;
            pdfSaveOptions.DisplayDocTitle = true;
            pdfSaveOptions.FontEncoding = PdfFontEncoding.Identity;
            pdfSaveOptions.EmbedAttachments = true;
            pdfSaveOptions.DefaultFont = &quot;Arial&quot;;
            pdfSaveOptions.CheckWorkbookDefaultFont = true;
            pdfSaveOptions.CheckFontCompatibility = true;
            pdfSaveOptions.IsFontSubstitutionCharGranularity = true;
            pdfSaveOptions.OnePagePerSheet = true;
            pdfSaveOptions.AllColumnsInOnePagePerSheet = true;
            pdfSaveOptions.IgnoreError = true;
            pdfSaveOptions.OutputBlankPageWhenNothingToPrint = true;
            pdfSaveOptions.PageIndex = 0;
            pdfSaveOptions.PageCount = 1;
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;
            pdfSaveOptions.GridlineType = GridlineType.Dotted;
            pdfSaveOptions.TextCrossType = TextCrossType.CrossKeep;
            pdfSaveOptions.DefaultEditLanguage = DefaultEditLanguage.English;
            pdfSaveOptions.SheetSet = SheetSet.Visible;
            pdfSaveOptions.ClearData = true;
            pdfSaveOptions.CachedFileFolder = &quot;C:\\Temp&quot;;
            pdfSaveOptions.ValidateMergedAreas = true;
            pdfSaveOptions.MergeAreas = true;
            pdfSaveOptions.SortNames = true;
            pdfSaveOptions.SortExternalNames = true;
            pdfSaveOptions.RefreshChartCache = true;

            // Set security options
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions
            {
                OwnerPassword = &quot;OwnerPassword&quot;,
                UserPassword = &quot;UserPassword&quot;,
                PrintPermission = true,
                FullQualityPrintPermission = true
            };
            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

            // Set watermark
            RenderingFont font = new RenderingFont(&quot;Calibri&quot;, 68)
            {
                Italic = true,
                Bold = true,
                Color = Color.Blue
            };
            RenderingWatermark watermark = new RenderingWatermark(&quot;Watermark&quot;, font)
            {
                HAlignment = TextAlignmentType.Center,
                VAlignment = TextAlignmentType.Center,
                Rotation = 30,
                Opacity = 0.6f,
                ScaleToPagePercent = 50
            };
            pdfSaveOptions.Watermark = watermark;

            // Save the workbook as a PDF file
            workbook.Save(&quot;PdfSaveOptionsExample.pdf&quot;, pdfSaveOptions);
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


