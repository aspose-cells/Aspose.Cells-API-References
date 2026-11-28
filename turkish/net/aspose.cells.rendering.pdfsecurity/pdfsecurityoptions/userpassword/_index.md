---
title: "PdfSecurityOptions.UserPassword"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSecurityOptions özelliği. Şifrelenmiş PDF belgesini açmak için gereken kullanıcı şifresini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/userpassword/
---
## PdfSecurityOptions.UserPassword property

Şifrelenmiş PDF belgesini açmak için gereken kullanıcı şifresini alır veya ayarlar.

```csharp
public string UserPassword { get; set; }
```

### Açıklamalar

Görünüm için şifrelenmiş bir PDF belgesini açmak üzere sahip şifresi veya kullanıcı şifresi gerekecektir.

Kullanıcı şifresi null ya da boş bir dize olabilir; bu durumda PDF belgesini açarken kullanıcıdan şifre istenmez.

Belgeyi doğru sahip şifresiyle açmak, belgeye tam erişim sağlar.

Belgeyi doğru kullanıcı şifresiyle (veya kullanıcı şifresi olmayan bir belgeyi) açmak, belirtilen izinler doğrultusunda sınırlı erişim sağlar.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyUserPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF with User Password";

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();
            
            securityOptions.UserPassword = "user123";
            securityOptions.OwnerPassword = "owner456";
            securityOptions.PrintPermission = true;
            
            saveOptions.SecurityOptions = securityOptions;
            workbook.Save("ProtectedWithUserPassword.pdf", saveOptions);
            
            Console.WriteLine("PDF created with user password protection.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


