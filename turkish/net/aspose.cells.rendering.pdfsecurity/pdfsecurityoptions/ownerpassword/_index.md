---
title: "PdfSecurityOptions.OwnerPassword"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSecurityOptions özelliği. Şifrelenmiş PDF belgesi için sahibi parolasını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/ownerpassword/
---
## PdfSecurityOptions.OwnerPassword property

Şifrelenmiş PDF belgesi için sahibi şifresini alır veya ayarlar.

```csharp
public string OwnerPassword { get; set; }
```

### Açıklamalar

Sahip şifresi, kullanıcının belirtilen herhangi bir erişim kısıtlaması olmadan şifrelenmiş bir PDF belgesini açmasına izin verir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyOwnerPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF with Owner Password";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.PrintPermission = true;
            securityOptions.ModifyDocumentPermission = false;

            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecuredPdfWithOwnerPassword.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with owner password protection.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


