---
title: "PdfSecurityOptions.ExtractContentPermission"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSecurityOptions özelliği. AccessibilityExtractContent tarafından kontrol edilen işlemler dışındaki işlemlerle belgeden metin ve grafik kopyalamaya veya çıkarmaya izin verilip verilmeyeceğini gösterir."
type: docs
url: /tr/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermission/
---
## PdfSecurityOptions.ExtractContentPermission property

Belgeden metin ve grafikleri kopyalamaya veya çıkarmaya izin verilip verilmeyeceğini, [`AccessibilityExtractContent`](../accessibilityextractcontent/) tarafından kontrol edilen işlemler dışındaki işlemlerle gösterir.

```csharp
public bool ExtractContentPermission { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyExtractContentPermissionDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Sample PDF Content";

            // PDF kaydetme seçeneklerini güvenlik ayarlarıyla yapılandırın
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            // Şifreleri ve izinleri ayarlayın
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            
            // ExtractContentPermission kullanımını gösterin
            securityOptions.ExtractContentPermission = false;
            securityOptions.PrintPermission = true;
            securityOptions.ModifyDocumentPermission = false;

            // Güvenlik seçeneklerini uygulayın ve kaydedin
            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecuredPDF.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with ExtractContentPermission set to false");
        }
    }
}
```

### Ayrıca Bakınız

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


