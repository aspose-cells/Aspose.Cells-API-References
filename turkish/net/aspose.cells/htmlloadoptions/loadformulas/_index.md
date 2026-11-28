---
title: "HtmlLoadOptions.LoadFormulas"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlLoadOptions özelliği. Orijinal html dosyası formüller içeriyorsa formüllerin içe aktarılıp aktarılmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/htmlloadoptions/loadformulas/
---
## HtmlLoadOptions.LoadFormulas property

Orijinal html dosyası formüller içeriyorsa formüllerin içe aktarılıp aktarılmayacağını gösterir.

```csharp
public bool LoadFormulas { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyLoadFormulasDemo
    {
        public static void Run()
        {
            // HtmlLoadOptions bir örnek oluştur.
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Formülleri HTML'den yüklemek için LoadFormulas'ı true olarak ayarlayın
            loadOptions.LoadFormulas = true;

            // Formüller içeren bir HTML dosyasını bir Çalışma Kitabı'na yükle
            Workbook workbook = new Workbook("input.html", loadOptions);

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresindeki formülü (HTML'de mevcutsa) görüntüle
            Console.WriteLine("Formula in A1: " + worksheet.Cells["A1"].Formula);

            // Çalışma kitabını bir Excel dosyasına kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


