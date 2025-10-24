##PdfSecurityOptions.ExtractContentPermissionObsolete
PdfSecurityOptions property. Permission to copy or extract content Obsoleted according to PDF reference
## PdfSecurityOptions.ExtractContentPermissionObsolete property
Permission to copy or extract content Obsoleted according to PDF reference.
```csharp
[Obsolete("Use ExtractContentPermission property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ExtractContentPermissionObsolete { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use ExtractContentPermission property. This property will be removed 12 months later since September 2023. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;
namespace AsposeCellsExamples
{
public class PdfSecurityOptionsPropertyExtractContentPermissionObsoleteDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
pdfSecurityOptions.OwnerPassword = "owner123";
pdfSecurityOptions.UserPassword = "user123";
pdfSecurityOptions.ExtractContentPermissionObsolete = false;
pdfSecurityOptions.ExtractContentPermission = true;
pdfSaveOptions.SecurityOptions = pdfSecurityOptions;
workbook.Save("SecurePDF.pdf", pdfSaveOptions);
Console.WriteLine("PDF created with ExtractContentPermissionObsolete set to false");
}
}
}
```
### See Also
* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)
