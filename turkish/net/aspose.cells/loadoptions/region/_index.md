---
title: "LoadOptions.Region"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Yüklenecek Workbook için kullanılan bölgesel ayarları alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/loadoptions/region/
---
## LoadOptions.Region property

Yüklenmek üzere olan Workbook için kullanılan bölgesel ayarları alır veya ayarlar.

```csharp
public CountryCode Region { get; set; }
```

### Açıklamalar

Bölgesel ayarlar, yazı tipleri, temalar vb. gibi çalışma kitabının bazı özelliklerini başlatmak için kullanılabilir. CSV, HTML, ... gibi metin tabanlı dosya formatları için bölgesel ayar, sayı biçimlerini algılamak ve hücrelerdeki metin değerlerini sayısal veya tarih‑zaman değerlerine ayrıştırmak için de kullanılacaktır. Bu ayar, daha sonra oluşturulan çalışma kitabı için korunur; yani çalışma kitabının [`Region`](../../workbooksettings/region/) özelliği bu özellik ile aynı bölgeyi kullanacaktır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyRegionDemo
    {
        public static void Run()
        {
            // HTML dosyası için yükleme seçenekleri oluştur
            LoadOptions loadOpts = new LoadOptions(LoadFormat.Html);
            
            // Bölgeyi USA olarak ayarla
            loadOpts.Region = CountryCode.USA;
            
            // HTML dosyasını belirtilen bölge ayarlarıyla yükle
            Workbook wb = new Workbook("example.html", loadOpts);
            
            // İlk çalışma sayfasına eriş
            Worksheet ws = wb.Worksheets[0];
            
            // Bir hücrenin stilini kontrol ederek bölgeye özgü biçimlendirmeyi göster
            Style style = ws.Cells["A1"].GetStyle();
            Console.WriteLine("Font used in cell A1: " + style.Font.Name);
            Console.WriteLine("Region used for loading: " + loadOpts.Region);
        }
    }
}
```

### Ayrıca Bakınız

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


