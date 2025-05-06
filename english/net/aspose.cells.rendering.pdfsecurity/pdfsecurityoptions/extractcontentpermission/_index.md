---
title: PdfSecurityOptions.ExtractContentPermission
second_title: Aspose.Cells for .NET API Reference
description: PdfSecurityOptions property. Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by AccessibilityExtractContent
type: docs
url: /net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermission/
---
## PdfSecurityOptions.ExtractContentPermission property

Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by [`AccessibilityExtractContent`](../accessibilityextractcontent/).

```csharp
public bool ExtractContentPermission { get; set; }
```

### Examples

```csharp
// Called: pdfSecurityOptions.ExtractContentPermission = false;
public static void Property_ExtractContentPermission()
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


