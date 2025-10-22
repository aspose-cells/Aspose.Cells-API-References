##PdfSecurityOptions.UserPassword
PdfSecurityOptions property. Gets or sets the user password required for opening the encrypted PDF document
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
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;
namespace AsposeCellsExamples
{
public class PdfSecurityOptionsPropertyUserPasswordDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF with User Password";
PdfSaveOptions saveOptions = new PdfSaveOptions();
PdfSecurityOptions securityOptions = new PdfSecurityOptions();
securityOptions.UserPassword = "user123";
securityOptions.OwnerPassword = "owner456";
securityOptions.PrintPermission = true;
saveOptions.SecurityOptions = securityOptions;
workbook.Save("ProtectedWithUserPassword.pdf", saveOptions);
Console.WriteLine("PDF created with user password protection.");
}
}
}
```
### See Also
* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)
