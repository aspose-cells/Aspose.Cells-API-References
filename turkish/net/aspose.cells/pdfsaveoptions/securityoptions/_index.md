---
title: SecurityOptions
second_title: Aspose.Cells for .NET API Referansı
description: xls2pdf sonucunda güvenlik gerektiğinde bu seçenekleri ayarlayın.
type: docs
weight: 300
url: /tr/net/aspose.cells/pdfsaveoptions/securityoptions/
---
## PdfSaveOptions.SecurityOptions property

xls2pdf sonucunda güvenlik gerektiğinde bu seçenekleri ayarlayın.

```csharp
public PdfSecurityOptions SecurityOptions { get; set; }
```

### Örnekler

Aşağıdaki kod, çıktı pdf için yüksek çözünürlüklü yazdırma iznini ayarlar.

```csharp
Workbook wb = new Workbook();
wb.Worksheets[0].Cells["A1"].Value = "Aspose";

PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();


PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

// sahip şifresini ayarla
pdfSecurityOptions.OwnerPassword = "YourOwnerPassword";

//Kullanıcı şifresini ayarla
pdfSecurityOptions.UserPassword = "YourUserPassword";

// yazdırma iznini ayarla
pdfSecurityOptions.PrintPermission = true;

//baskı için yüksek çözünürlüğü ayarla
pdfSecurityOptions.FullQualityPrintPermission = true;


pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

wb.Save("output.pdf", pdfSaveOptions);
```

### Ayrıca bakınız

* class [PdfSecurityOptions](../../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions)
* class [PdfSaveOptions](../../pdfsaveoptions)
* ad alanı [Aspose.Cells](../../pdfsaveoptions)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
