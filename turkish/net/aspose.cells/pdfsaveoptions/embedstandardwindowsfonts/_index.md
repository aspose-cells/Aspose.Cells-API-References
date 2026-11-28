---
title: "PdfSaveOptions.EmbedStandardWindowsFonts"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSaveOptions özelliği. True, TrueType yazı tiplerini gömmek için. Yalnızca ASCII karakterleri 32127 etkiler. 127'den büyük karakter kodları için yazı tipleri her zaman gömülür. PDF/A1a PDF/A1b standardı için yazı tipleri her zaman gömülür. Varsayılan değer true'dur."
type: docs
url: /tr/net/aspose.cells/pdfsaveoptions/embedstandardwindowsfonts/
---
## PdfSaveOptions.EmbedStandardWindowsFonts property

True, gerçek tip (TrueType) yazı tiplerini gömmek için. Yalnızca ASCII karakterleri 32-127 etkiler. 127'den büyük karakter kodları için yazı tipleri her zaman gömülür. PDF/A-1a, PDF/A-1b standartları için yazı tipleri her zaman gömülür. Varsayılan değer true'dur.

```csharp
public bool EmbedStandardWindowsFonts { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyEmbedStandardWindowsFontsDemo
    {
        public static void Run()
        {
            // Örnek bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test PDF with embedded fonts");

            // EmbedStandardWindowsFonts özelliği ile PDF kaydetme seçeneklerini ayarla
            PdfSaveOptions options = new PdfSaveOptions();
            options.EmbedStandardWindowsFonts = true;

            // Bellek akışına kaydet
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, options);
                Console.WriteLine("PDF saved with embedded fonts: " + (ms.Length > 0));
            }

            // Yazı tipi gömme işlemini devre dışı bırakmayı göster
            options.EmbedStandardWindowsFonts = false;
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, options);
                Console.WriteLine("PDF saved without embedded fonts: " + (ms.Length > 0));
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


