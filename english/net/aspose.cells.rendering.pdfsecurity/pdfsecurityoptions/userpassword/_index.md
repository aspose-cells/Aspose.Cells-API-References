---
title: PdfSecurityOptions.UserPassword
second_title: Aspose.Cells for .NET API Reference
description: PdfSecurityOptions property. Gets or sets the user password required for opening the encrypted PDF document
type: docs
url: /net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/userpassword/
---
## PdfSecurityOptions.UserPassword property

Gets or sets the user password required for opening the encrypted PDF document.

```csharp
public string UserPassword { get; set; }
```

### Remarks

The owner password or user password will be required to open an encrypted PDF document for viewing.

The user password can be null or empty string, in this case no password will be required from the user when opening the PDF document.

Opening the document with the correct owner password allows full access to the document.

Opening the document with the correct user password (or opening a document that does not have a user password) allows limited access as the permissions specified.

### Examples

```csharp
// Called: pdfSecurityOptions.UserPassword = "YourUserPassword";
public static void PdfSecurityOptions_Property_UserPassword()
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


