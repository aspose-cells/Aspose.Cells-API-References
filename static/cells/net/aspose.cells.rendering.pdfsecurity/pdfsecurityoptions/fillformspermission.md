##PdfSecurityOptions.FillFormsPermission
PdfSecurityOptions property. Indicates whether to allow to fill in existing interactive form fields including signature fields even if ModifyDocumentPermission is clear
## PdfSecurityOptions.FillFormsPermission property
Indicates whether to allow to fill in existing interactive form fields (including signature fields), even if [`ModifyDocumentPermission`](../modifydocumentpermission/) is clear.
```csharp
public bool FillFormsPermission { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;
namespace AsposeCellsExamples
{
public class PdfSecurityOptionsPropertyFillFormsPermissionDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].Value = "PDF Form Example";
// Configure PDF save options with security settings
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
PdfSecurityOptions securityOptions = new PdfSecurityOptions();
// Set passwords and permissions
securityOptions.OwnerPassword = "owner123";
securityOptions.UserPassword = "user123";
securityOptions.FillFormsPermission = true; // Key permission being demonstrated
securityOptions.PrintPermission = true;
// Apply security options and save
pdfSaveOptions.SecurityOptions = securityOptions;
workbook.Save("SecureFormFillEnabled.pdf", pdfSaveOptions);
Console.WriteLine("PDF created with form filling permission enabled.");
}
}
}
```
### See Also
* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)
