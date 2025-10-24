##PdfSecurityOptions.FullQualityPrintPermission
PdfSecurityOptions property. Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated
## PdfSecurityOptions.FullQualityPrintPermission property
Indicates whether to allow to print the document to a representation from which a faithful digital copy of the PDF content could be generated.
```csharp
public bool FullQualityPrintPermission { get; set; }
```
### Remarks
When it is clear (and [`PrintPermission`](../printpermission/) is set), printing is limited to a low level representation of the appearance, possibly of degraded quality.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;
namespace AsposeCellsExamples
{
public class PdfSecurityOptionsPropertyFullQualityPrintPermissionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].Value = "Test Full Quality Print Permission";
PdfSaveOptions saveOptions = new PdfSaveOptions();
PdfSecurityOptions securityOptions = new PdfSecurityOptions();
securityOptions.OwnerPassword = "owner123";
securityOptions.UserPassword = "user123";
securityOptions.FullQualityPrintPermission = true;
securityOptions.PrintPermission = true;
saveOptions.SecurityOptions = securityOptions;
workbook.Save("FullQualityPrintDemo.pdf", saveOptions);
Console.WriteLine("PDF created with FullQualityPrintPermission enabled.");
}
}
}
```
### See Also
* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)
