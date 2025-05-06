---
title: PdfSecurityOptions.FullQualityPrintPermission
second_title: Aspose.Cells for .NET API Reference
description: PdfSecurityOptions property. Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated
type: docs
url: /net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fullqualityprintpermission/
---
## PdfSecurityOptions.FullQualityPrintPermission property

Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated.

```csharp
public bool FullQualityPrintPermission { get; set; }
```

### Remarks

When it is clear (and [`PrintPermission`](../printpermission/) is set), printing is limited to a low level representation of the appearance, possibly of degraded quality.

### Examples

```csharp
// Called: pdfSecurityOptions.FullQualityPrintPermission = true;
public static void Property_FullQualityPrintPermission()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells[&quot;A1&quot;].Value = &quot;Aspose&quot;;

            // Create PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Create PdfSecurityOptions
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            // Set security options
            pdfSecurityOptions.OwnerPassword = &quot;YourOwnerPassword&quot;;
            pdfSecurityOptions.UserPassword = &quot;YourUserPassword&quot;;
            pdfSecurityOptions.PrintPermission = true;
            pdfSecurityOptions.ModifyDocumentPermission = false;
            pdfSecurityOptions.ExtractContentPermissionObsolete = false;
            pdfSecurityOptions.AnnotationsPermission = true;
            pdfSecurityOptions.FillFormsPermission = true;
            pdfSecurityOptions.ExtractContentPermission = false;
            pdfSecurityOptions.AccessibilityExtractContent = true;
            pdfSecurityOptions.AssembleDocumentPermission = false;
            pdfSecurityOptions.FullQualityPrintPermission = true;

            // Assign security options to PdfSaveOptions
            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

            // Save the workbook as a PDF with the specified security options
            workbook.Save(&quot;output.pdf&quot;, pdfSaveOptions);
        }
```

### See Also

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


