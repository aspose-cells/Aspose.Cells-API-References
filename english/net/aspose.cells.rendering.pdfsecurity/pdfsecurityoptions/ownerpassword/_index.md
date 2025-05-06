---
title: PdfSecurityOptions.OwnerPassword
second_title: Aspose.Cells for .NET API Reference
description: PdfSecurityOptions property. Gets or sets the owner password for the encrypted PDF document
type: docs
url: /net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/ownerpassword/
---
## PdfSecurityOptions.OwnerPassword property

Gets or sets the owner password for the encrypted PDF document.

```csharp
public string OwnerPassword { get; set; }
```

### Remarks

The owner password allows the user to open an encrypted PDF document without any access restrictions specified.

### Examples

```csharp
// Called: OwnerPassword = &amp;quot;OwnerPassword&amp;quot;,
public static void Property_OwnerPassword()
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

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


