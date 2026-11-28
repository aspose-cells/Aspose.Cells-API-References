---
title: "PaginatedSaveOptions.CheckFontCompatibility"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PaginatedSaveOptions özelliği. Metindeki her karakter için yazı tipi uyumluluğunu kontrol edip etmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/paginatedsaveoptions/checkfontcompatibility/
---
## PaginatedSaveOptions.CheckFontCompatibility property

Metindeki her karakter için yazı tipi uyumluluğunun kontrol edilip edilmeyeceğini gösterir.

```csharp
public bool CheckFontCompatibility { get; set; }
```

### Açıklamalar

Varsayılan değer true'dur. Bu özelliği devre dışı bırakmak daha iyi performans sağlayabilir. Ancak metnin/karakterin varsayılan veya belirtilen yazı tipi render edilemediğinde, oluşturulan pdf'de okunamayan karakterler (örneğin blok) ortaya çıkabilir. Böyle bir durumda kullanıcı bu özelliği true olarak tutmalıdır, böylece alternatif bir yazı tipi aranıp metni render etmek için kullanılabilir;

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyCheckFontCompatibilityDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Font Compatibility Test");

            // Sayfalı kaydetme seçenekleri oluşturun
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // CheckFontCompatibility özelliğini gösterin
            saveOptions.CheckFontCompatibility = false; // Disable font compatibility checking
            
            // Diğer gerekli özellikleri ayarlayın
            saveOptions.DefaultFont = "Arial";
            saveOptions.CheckWorkbookDefaultFont = true;

            // Belirtilen seçeneklerle belgeyi kaydedin
            workbook.Save("PaginatedSaveOptions_CheckFontCompatibility.pdf", saveOptions);
            
            Console.WriteLine("Document saved with CheckFontCompatibility = false");
        }
    }
}
```

### Ayrıca Bakınız

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


