---
title: "PdfSaveOptions.FontEncoding"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSaveOptions özelliği. PDF içinde gömülü yazı tipi kodlamasını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/pdfsaveoptions/fontencoding/
---
## PdfSaveOptions.FontEncoding property

PDF içinde gömülü yazı tipi kodlamasını alır veya ayarlar.

```csharp
public PdfFontEncoding FontEncoding { get; set; }
```

### Açıklamalar

Varsayılan değer Identity'dir

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyFontEncodingDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Font Encoding Test");
            worksheet.Cells["A2"].PutValue("This demonstrates PdfFontEncoding usage");

            // Yazı tipi kodlamasıyla PDF kaydetme seçeneklerini yapılandırın
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.FontEncoding = PdfFontEncoding.Identity;
            pdfSaveOptions.DefaultFont = "Arial";

            // Çalışma kitabını PDF olarak kaydedin
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* enum [PdfFontEncoding](../../../aspose.cells.rendering/pdffontencoding/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


