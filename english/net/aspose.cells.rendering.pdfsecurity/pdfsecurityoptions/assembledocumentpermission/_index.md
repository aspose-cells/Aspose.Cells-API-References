---
title: PdfSecurityOptions.AssembleDocumentPermission
second_title: Aspose.Cells for .NET API Reference
description: PdfSecurityOptions property. Indicates whether to allow to assemble the document insert rotate or delete pages and create bookmarks or thumbnail images even if ModifyDocumentPermission is clear
type: docs
url: /net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/assembledocumentpermission/
---
## PdfSecurityOptions.AssembleDocumentPermission property

Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if [`ModifyDocumentPermission`](../modifydocumentpermission/) is clear.

```csharp
public bool AssembleDocumentPermission { get; set; }
```

### Examples

```csharp
// Called: pdfSecurityOptions.AssembleDocumentPermission = false;
public static void Property_AssembleDocumentPermission()
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


