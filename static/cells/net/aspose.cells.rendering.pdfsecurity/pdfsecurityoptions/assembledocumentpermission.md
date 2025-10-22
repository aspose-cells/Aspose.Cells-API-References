##PdfSecurityOptions.AssembleDocumentPermission
PdfSecurityOptions property. Indicates whether to allow to assemble the document insert rotate or delete pages and create bookmarks or thumbnail images even if ModifyDocumentPermission is clear
## PdfSecurityOptions.AssembleDocumentPermission property
Indicates whether to allow to assemble the document (insert, rotate, or delete pages and create bookmarks or thumbnail images), even if [`ModifyDocumentPermission`](../modifydocumentpermission/) is clear.
```csharp
public bool AssembleDocumentPermission { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;
namespace AsposeCellsExamples
{
public class PdfSecurityOptionsPropertyAssembleDocumentPermissionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
pdfSecurityOptions.OwnerPassword = "owner123";
pdfSecurityOptions.UserPassword = "user123";
pdfSecurityOptions.AssembleDocumentPermission = false;
pdfSecurityOptions.PrintPermission = true;
pdfSaveOptions.SecurityOptions = pdfSecurityOptions;
workbook.Save("secured_document.pdf", pdfSaveOptions);
Console.WriteLine("PDF created with assemble document permission disabled.");
}
}
}
```
### See Also
* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)
