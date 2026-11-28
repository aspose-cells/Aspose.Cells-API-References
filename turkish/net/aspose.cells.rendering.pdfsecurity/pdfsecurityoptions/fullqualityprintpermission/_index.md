---
title: "PdfSecurityOptions.FullQualityPrintPermission"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSecurityOptions özelliği. Belgenin, PDF içeriğinin doğru bir dijital kopyasının oluşturulabileceği bir temsile yazdırılmasına izin verilip verilmediğini gösterir."
type: docs
url: /tr/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fullqualityprintpermission/
---
## PdfSecurityOptions.FullQualityPrintPermission property

PDF içeriğinin doğru bir dijital kopyası oluşturulabilecek bir temsile belgeyi yazdırmaya izin verilip verilmediğini gösterir.

```csharp
public bool FullQualityPrintPermission { get; set; }
```

### Açıklamalar

Bu ayar açık olduğunda (ve [`PrintPermission`](../printpermission/) ayarlanmışsa), yazdırma, görünümün düşük seviyeli bir temsiliyle, muhtemelen bozulmuş kaliteyle sınırlıdır.

### Örnekler

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

### Ayrıca Bakınız

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


