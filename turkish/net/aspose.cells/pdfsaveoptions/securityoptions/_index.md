---
title: "PdfSaveOptions.SecurityOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSaveOptions özelliği. xls2pdf sonucunda güvenlik gerektiğinde bu seçenekleri ayarlayın"
type: docs
url: /tr/net/aspose.cells/pdfsaveoptions/securityoptions/
---
## PdfSaveOptions.SecurityOptions property

Güvenliğin xls2pdf sonucunda gerektiği durumlarda bu seçenekleri ayarlayın.

```csharp
public PdfSecurityOptions SecurityOptions { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertySecurityOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Örnek veri ekleyin.
            workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF Demo";
            
            // PDF kaydetme seçeneklerini oluşturun
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Güvenlik seçeneklerini yapılandırın
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.PrintPermission = true;
            securityOptions.ModifyDocumentPermission = false;
            securityOptions.ExtractContentPermission = false;
            
            // Güvenlik seçeneklerini kaydetme seçeneklerine atayın
            saveOptions.SecurityOptions = securityOptions;
            
            // PDF'yi güvenlik ayarlarıyla kaydedin
            workbook.Save("SecuredDocument.pdf", saveOptions);
            
            Console.WriteLine("PDF with security options created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PdfSecurityOptions](../../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


