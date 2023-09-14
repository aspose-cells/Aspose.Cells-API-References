---
title: PdfSecurityOptions.PdfSecurityOptions
second_title: Aspose.Cells for .NET API Reference
description: PdfSecurityOptions constructor. The constructor of PdfSecurityOptions
type: docs
url: /net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/pdfsecurityoptions/
---
## PdfSecurityOptions constructor

The constructor of PdfSecurityOptions

```csharp
public PdfSecurityOptions()
```

### Examples

The following code sets high resolution print permisson for the output pdf.

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

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


