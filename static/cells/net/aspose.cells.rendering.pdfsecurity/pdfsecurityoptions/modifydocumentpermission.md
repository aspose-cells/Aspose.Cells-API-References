##PdfSecurityOptions.ModifyDocumentPermission
PdfSecurityOptions property. Indicates whether to allow to modify the contents of the document by operations other than those controlled by AnnotationsPermission FillFormsPermission and AssembleDocumentPermission
## PdfSecurityOptions.ModifyDocumentPermission property
Indicates whether to allow to modify the contents of the document by operations other than those controlled by [`AnnotationsPermission`](../annotationspermission/), [`FillFormsPermission`](../fillformspermission/) and [`AssembleDocumentPermission`](../assembledocumentpermission/).
```csharp
public bool ModifyDocumentPermission { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;
namespace AsposeCellsExamples
{
public class PdfSecurityOptionsPropertyModifyDocumentPermissionDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";
// Configure PDF save options with security settings
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
PdfSecurityOptions securityOptions = new PdfSecurityOptions();
// Set passwords and permissions
securityOptions.OwnerPassword = "owner123";
securityOptions.UserPassword = "user123";
securityOptions.ModifyDocumentPermission = false; // Core property demonstration
securityOptions.PrintPermission = true;
// Apply security options and save
pdfSaveOptions.SecurityOptions = securityOptions;
workbook.Save("SecuredDocument.pdf", pdfSaveOptions);
Console.WriteLine("PDF created with ModifyDocumentPermission set to false");
}
}
}
```
### See Also
* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)
