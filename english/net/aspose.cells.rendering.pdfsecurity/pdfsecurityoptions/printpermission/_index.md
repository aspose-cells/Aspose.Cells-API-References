---
title: PdfSecurityOptions.PrintPermission
second_title: Aspose.Cells for .NET API Reference
description: PdfSecurityOptions property. Indicates whether to allow to print the document
type: docs
url: /net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/printpermission/
---
## PdfSecurityOptions.PrintPermission property

Indicates whether to allow to print the document.

```csharp
public bool PrintPermission { get; set; }
```

### Remarks

Possibly not at the highest quality level, depending on whether [`FullQualityPrintPermission`](../fullqualityprintpermission/) is also set.

### Examples

```csharp
// Called: pdfSecurityOptions.PrintPermission = true;
public static void Property_PrintPermission()
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


