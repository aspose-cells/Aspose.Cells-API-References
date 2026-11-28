---
title: "PdfSaveOptions.Compliance"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSaveOptions özelliği. Çıktı belgeleri için PDF standartları uyumluluk seviyesini alır veya ayarlar."
type: docs
url: /tr/net/aspose.cells/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

Çıktı belgeleri için PDF standartları uyumluluk seviyesini alır veya ayarlar.

```csharp
public PdfCompliance Compliance { get; set; }
```

### Açıklamalar

Varsayılan değer Pdf17'dir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyComplianceDemo
    {
        public static void Run()
        {
            // Test verileriyle örnek bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test PDF Compliance");

            // PDF/A-1b uyumluluğu ile PDF kaydetme seçeneklerini ayarla
            PdfSaveOptions options = new PdfSaveOptions
            {
                Compliance = PdfCompliance.PdfA1b
            };

            // Çalışma kitabını uyumluluk ayarlarıyla PDF olarak kaydet
            workbook.Save("output.pdf", options);
            
            Console.WriteLine("PDF saved with PDF/A-1b compliance.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PdfCompliance](../../../aspose.cells.rendering/pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


