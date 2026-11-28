---
title: "HtmlSaveOptions.SaveAsSingleFile"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. HTML'nin tek dosya olarak kaydedilip kaydedilmeyeceğini gösterir. Varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/saveassinglefile/
---
## HtmlSaveOptions.SaveAsSingleFile property

HTML'nin tek dosya olarak kaydedilip kaydedilmeyeceğini gösterir. Varsayılan değer false'tur.

```csharp
public bool SaveAsSingleFile { get; set; }
```

### Açıklamalar

Çalışma kitabında birden fazla çalışma sayfası veya resimler gibi diğer gerekli kaynaklar varsa, genellikle bu çalışma sayfaları ve diğer kaynaklar ayrı dosyalara kaydedilir. Bazı senaryolarda, kullanıcı taşıma kolaylığı gibi tek bir sonuç dosyası elde etmek isteyebilir. Böyle bir durumda, kullanıcı bu özelliği true olarak ayarlayabilir.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertySaveAsSingleFileDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // HTML kaydetme seçeneklerini başlatın
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.SaveAsSingleFile = true;
            saveOptions.ExportPageHeaders = true;
            
            // Çalışma kitabını tek HTML dosyası olarak kaydedin
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            // Çıktı dosyasının var olduğunu doğrulayın
            if (File.Exists(outputPath))
            {
                Console.WriteLine("HTML saved as single file successfully.");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


