##PdfSecurityOptions.OwnerPassword
PdfSecurityOptions property. Gets or sets the owner password for the encrypted PDF document
## PdfSecurityOptions.OwnerPassword property
Gets or sets the owner password for the encrypted PDF document.
```csharp
public string OwnerPassword { get; set; }
```
### Remarks
The owner password allows the user to open an encrypted PDF document without any access restrictions specified.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;
namespace AsposeCellsExamples
{
public class PdfSecurityOptionsPropertyOwnerPasswordDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF with Owner Password";
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
PdfSecurityOptions securityOptions = new PdfSecurityOptions();
securityOptions.OwnerPassword = "owner123";
securityOptions.UserPassword = "user123";
securityOptions.PrintPermission = true;
securityOptions.ModifyDocumentPermission = false;
pdfSaveOptions.SecurityOptions = securityOptions;
workbook.Save("SecuredPdfWithOwnerPassword.pdf", pdfSaveOptions);
Console.WriteLine("PDF created with owner password protection.");
}
}
}
```
### See Also
* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)
