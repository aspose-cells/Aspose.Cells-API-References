##PdfSecurityOptions.ExtractContentPermission
PdfSecurityOptions property. Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by AccessibilityExtractContent
## PdfSecurityOptions.ExtractContentPermission property
Indicates whether to allow to copy or otherwise extract text and graphics from the document by operations other than that controlled by [`AccessibilityExtractContent`](../accessibilityextractcontent/).
```csharp
public bool ExtractContentPermission { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;
namespace AsposeCellsExamples
{
public class PdfSecurityOptionsPropertyExtractContentPermissionDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].Value = "Sample PDF Content";
// Configure PDF save options with security settings
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
PdfSecurityOptions securityOptions = new PdfSecurityOptions();
// Set passwords and permissions
securityOptions.OwnerPassword = "owner123";
securityOptions.UserPassword = "user123";
// Demonstrate ExtractContentPermission usage
securityOptions.ExtractContentPermission = false;
securityOptions.PrintPermission = true;
securityOptions.ModifyDocumentPermission = false;
// Apply security options and save
pdfSaveOptions.SecurityOptions = securityOptions;
workbook.Save("SecuredPDF.pdf", pdfSaveOptions);
Console.WriteLine("PDF created with ExtractContentPermission set to false");
}
}
}
```
### See Also
* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)
