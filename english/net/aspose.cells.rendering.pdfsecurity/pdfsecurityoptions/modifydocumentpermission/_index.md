---
title: PdfSecurityOptions.ModifyDocumentPermission
second_title: Aspose.Cells for .NET API Reference
description: PdfSecurityOptions property. Indicates whether to allow to modify the contents of the document by operations other than those controlled by AnnotationsPermission FillFormsPermission and AssembleDocumentPermission
type: docs
url: /net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/modifydocumentpermission/
---
## PdfSecurityOptions.ModifyDocumentPermission property

Indicates whether to allow to modify the contents of the document by operations other than those controlled by [`AnnotationsPermission`](../annotationspermission/), [`FillFormsPermission`](../fillformspermission/) and [`AssembleDocumentPermission`](../assembledocumentpermission/).

```csharp
public bool ModifyDocumentPermission { get; set; }
```

### Examples

```csharp
// Called: pdfSecurityOptions.ModifyDocumentPermission = false;
public static void PdfSecurityOptions_Property_ModifyDocumentPermission()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Aspose";

            // Create PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Create PdfSecurityOptions
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            // Set security options
            pdfSecurityOptions.OwnerPassword = "YourOwnerPassword";
            pdfSecurityOptions.UserPassword = "YourUserPassword";
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
            workbook.Save("output.pdf", pdfSaveOptions);
        }
```

### See Also

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


