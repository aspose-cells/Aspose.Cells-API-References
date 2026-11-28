---
title: "LoadOptions.CultureInfo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Yüklenecek Workbook için kullanılan bölgesel ayarları alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/loadoptions/cultureinfo/
---
## LoadOptions.CultureInfo property

Yüklenmek üzere olan Workbook için kullanılan bölgesel ayarları alır veya ayarlar.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### Açıklamalar

Bu özelliğin, bölgesel ayarları belirlemek için [`Region`](../region/) ile aynı etkisi vardır.

### Örnekler

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCultureInfoDemo
    {
        public static void Run()
        {
            // Örnek Excel dosyası oluştur
            Workbook sampleWorkbook = new Workbook();
            sampleWorkbook.Worksheets[0].Cells["A1"].PutValue(1234.56);
            sampleWorkbook.Save("sample.xlsx", SaveFormat.Xlsx);

            // Belirli bir kültürle yükle
            LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
            options.CultureInfo = new CultureInfo("de-DE"); // German culture uses comma as decimal separator
            
            Workbook workbook = new Workbook("sample.xlsx", options);
            Console.WriteLine("Value with German culture: " + workbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


