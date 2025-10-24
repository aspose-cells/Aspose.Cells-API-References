##PdfSecurityOptions.AccessibilityExtractContent
PdfSecurityOptions property. Indicates whether to allow to extract text and graphics in support of accessibility to users with disabilities or for other purposes
## PdfSecurityOptions.AccessibilityExtractContent property
Indicates whether to allow to extract text and graphics (in support of accessibility to users with disabilities or for other purposes).
```csharp
public bool AccessibilityExtractContent { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;
namespace AsposeCellsExamples
{
public class PdfSecurityOptionsPropertyAccessibilityExtractContentDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].Value = "Test Accessibility Extract Content";
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
pdfSecurityOptions.OwnerPassword = "owner123";
pdfSecurityOptions.UserPassword = "user123";
pdfSecurityOptions.AccessibilityExtractContent = true;
pdfSecurityOptions.ExtractContentPermission = false;
pdfSaveOptions.SecurityOptions = pdfSecurityOptions;
workbook.Save("AccessibilityExtractContentDemo.pdf", pdfSaveOptions);
}
}
}
```
### See Also
* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)
