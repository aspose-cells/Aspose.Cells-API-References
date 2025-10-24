##PdfSecurityOptions.AnnotationsPermission
PdfSecurityOptions property. Indicates whether to allow to add or modify text annotations fill in interactive form fields
## PdfSecurityOptions.AnnotationsPermission property
Indicates whether to allow to add or modify text annotations, fill in interactive form fields.
```csharp
public bool AnnotationsPermission { get; set; }
```
### Remarks
if [`ModifyDocumentPermission`](../modifydocumentpermission/) is also set, create or modify interactive form fields (including signature fields).
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;
namespace AsposeCellsExamples
{
public class PdfSecurityOptionsPropertyAnnotationsPermissionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].Value = "Test PDF with Annotations Permission";
PdfSaveOptions saveOptions = new PdfSaveOptions();
PdfSecurityOptions securityOptions = new PdfSecurityOptions();
securityOptions.OwnerPassword = "owner123";
securityOptions.UserPassword = "user123";
securityOptions.AnnotationsPermission = true;
saveOptions.SecurityOptions = securityOptions;
workbook.Save("AnnotationsPermissionDemo.pdf", saveOptions);
Console.WriteLine("PDF created with annotations permission enabled.");
}
}
}
```
### See Also
* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)
