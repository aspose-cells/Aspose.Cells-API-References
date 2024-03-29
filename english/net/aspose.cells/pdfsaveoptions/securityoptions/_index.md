---
title: PdfSaveOptions.SecurityOptions
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions property. Set this options when security is need in xls2pdf result
type: docs
url: /net/aspose.cells/pdfsaveoptions/securityoptions/
---
## PdfSaveOptions.SecurityOptions property

Set this options, when security is need in xls2pdf result.

```csharp
public PdfSecurityOptions SecurityOptions { get; set; }
```

### Examples

The following code sets hight resolution print permisson for the output pdf.

```csharp
Workbook wb = new Workbook();
wb.Worksheets[0].Cells["A1"].Value = "Aspose";

PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();


PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

//set owner password
pdfSecurityOptions.OwnerPassword = "YourOwnerPassword";

//set user password
pdfSecurityOptions.UserPassword = "YourUserPassword";

//set print permisson
pdfSecurityOptions.PrintPermission = true;

//set high resolution for print
pdfSecurityOptions.FullQualityPrintPermission = true;


pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

wb.Save("output.pdf", pdfSaveOptions);
```

### See Also

* class [PdfSecurityOptions](../../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


