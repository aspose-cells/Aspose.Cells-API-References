---
title: "HtmlLoadOptions.AutoFitColsAndRows"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlLoadOptions özelliği. Sütun ve satırların otomatik olarak sığdırılıp sığdırılmayacağını gösterir. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/htmlloadoptions/autofitcolsandrows/
---
## HtmlLoadOptions.AutoFitColsAndRows property

Sütun ve satırların otomatik sığdırılıp sığdırılmayacağını gösterir. Varsayılan değer false'tur.

```csharp
public bool AutoFitColsAndRows { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyAutoFitColsAndRowsDemo
    {
        public static void Run()
        {
            // HTML yükleme seçenekleri oluştur
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            
            // Sütun ve satırların otomatik sığdırılmasını etkinleştirin
            loadOptions.AutoFitColsAndRows = true;
            
            // Belirtilen seçeneklerle HTML dosyasını yükleyin
            Workbook workbook = new Workbook("example.html", loadOptions);
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Yükleme sırasında sütun ve satırların otomatik sığdırılması uygulanacaktır
            Console.WriteLine("Columns and rows have been auto-fitted during HTML import.");
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


