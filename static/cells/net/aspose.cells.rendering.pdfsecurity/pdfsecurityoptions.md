##Class PdfSecurityOptions
Aspose.Cells.Rendering.PdfSecurity.PdfSecurityOptions class. Options for encrypting and access permissions for a PDF document. PDF/A does not allow security setting
## PdfSecurityOptions class
Options for encrypting and access permissions for a PDF document. PDF/A does not allow security setting.
```csharp
public class PdfSecurityOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [PdfSecurityOptions](pdfsecurityoptions/)() | The constructor of PdfSecurityOptions |
## Properties
| Name | Description |
| --- | --- |
| [AccessibilityExtractContent](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/accessibilityextractcontent/) { get; set; } | Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes). |
| [AnnotationsPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/annotationspermission/) { get; set; } | Indicates whether to allow to add or modify text annotations, fill in interactive form fields. |
| [AssembleDocumentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/assembledocumentpermission/) { get; set; } | Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if [`ModifyDocumentPermission`](./modifydocumentpermission/) is clear. |
| [ExtractContentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermission/) { get; set; } | Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by [`AccessibilityExtractContent`](./accessibilityextractcontent/). |
| [ExtractContentPermissionObsolete](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermissionobsolete/) { get; set; } | (**Obsolete.**) Permission to copy or extract content Obsoleted according to PDF reference. |
| [FillFormsPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fillformspermission/) { get; set; } | Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if [`ModifyDocumentPermission`](./modifydocumentpermission/) is clear. |
| [FullQualityPrintPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fullqualityprintpermission/) { get; set; } | Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated. |
| [ModifyDocumentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/modifydocumentpermission/) { get; set; } | Indicates whether to allow to modify the contents of the document by operations other than those controlled by [`AnnotationsPermission`](./annotationspermission/), [`FillFormsPermission`](./fillformspermission/) and [`AssembleDocumentPermission`](./assembledocumentpermission/). |
| [OwnerPassword](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/ownerpassword/) { get; set; } | Gets or sets the owner password for the encrypted PDF document. |
| [PrintPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/printpermission/) { get; set; } | Indicates whether to allow to print the document. |
| [UserPassword](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/userpassword/) { get; set; } | Gets or sets the user password required for opening the encrypted PDF document. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Rendering.PdfSecurity;
using System;
public class PdfSecurityOptionsDemo
{
public static void PdfSecurityOptionsExample()
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
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../)
