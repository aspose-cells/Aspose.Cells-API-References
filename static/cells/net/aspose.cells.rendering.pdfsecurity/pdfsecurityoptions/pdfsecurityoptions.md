##PdfSecurityOptions.PdfSecurityOptions
PdfSecurityOptions constructor. The constructor of PdfSecurityOptions
## PdfSecurityOptions constructor
The constructor of PdfSecurityOptions
```csharp
public PdfSecurityOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;
namespace AsposeCellsExamples
{
public class PdfSecurityOptionsMethodCtorDemo
{
public static void Run()
{
Workbook wb = new Workbook();
wb.Worksheets[0].Cells["A1"].Value = "Aspose PDF Security Demo";
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
// Using #ctor to create PdfSecurityOptions instance
PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
pdfSecurityOptions.OwnerPassword = "owner123";
pdfSecurityOptions.UserPassword = "user123";
pdfSecurityOptions.PrintPermission = true;
pdfSecurityOptions.FullQualityPrintPermission = true;
pdfSaveOptions.SecurityOptions = pdfSecurityOptions;
wb.Save("SecuredOutput.pdf", pdfSaveOptions);
Console.WriteLine("PDF with security options created successfully.");
}
}
}
```
### See Also
* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)
