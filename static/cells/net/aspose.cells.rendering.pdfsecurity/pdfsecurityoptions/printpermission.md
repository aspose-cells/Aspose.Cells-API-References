##PdfSecurityOptions.PrintPermission
PdfSecurityOptions property. Indicates whether to allow to print the document
## PdfSecurityOptions.PrintPermission property
Indicates whether to allow to print the document.
```csharp
public bool PrintPermission { get; set; }
```
### Remarks
Possibly not at the highest quality level, depending on whether [`FullQualityPrintPermission`](../fullqualityprintpermission/) is also set.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;
namespace AsposeCellsExamples
{
public class PdfSecurityOptionsPropertyPrintPermissionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].Value = "Test Print Permission";
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
PdfSecurityOptions securityOptions = new PdfSecurityOptions();
securityOptions.OwnerPassword = "owner123";
securityOptions.UserPassword = "user123";
securityOptions.PrintPermission = true;
pdfSaveOptions.SecurityOptions = securityOptions;
workbook.Save("PrintPermissionDemo.pdf", pdfSaveOptions);
Console.WriteLine("PDF created with print permission enabled.");
}
}
}
```
### See Also
* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)
