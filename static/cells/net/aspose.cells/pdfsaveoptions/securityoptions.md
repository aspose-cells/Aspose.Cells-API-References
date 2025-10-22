##PdfSaveOptions.SecurityOptions
PdfSaveOptions property. Set this options when security is need in xls2pdf result
## PdfSaveOptions.SecurityOptions property
Set this options, when security is need in xls2pdf result.
```csharp
public PdfSecurityOptions SecurityOptions { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;
namespace AsposeCellsExamples
{
public class PdfSaveOptionsPropertySecurityOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add sample data
workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF Demo";
// Create PDF save options
PdfSaveOptions saveOptions = new PdfSaveOptions();
// Configure security options
PdfSecurityOptions securityOptions = new PdfSecurityOptions();
securityOptions.OwnerPassword = "owner123";
securityOptions.UserPassword = "user123";
securityOptions.PrintPermission = true;
securityOptions.ModifyDocumentPermission = false;
securityOptions.ExtractContentPermission = false;
// Assign security options to save options
saveOptions.SecurityOptions = securityOptions;
// Save the PDF with security settings
workbook.Save("SecuredDocument.pdf", saveOptions);
Console.WriteLine("PDF with security options created successfully.");
}
}
}
```
### See Also
* class [PdfSecurityOptions](../../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
