---
title: "XmlLoadOptions.StartCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XmlLoadOptions özelliği. Başlangıç hücresini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/xmlloadoptions/startcell/
---
## XmlLoadOptions.StartCell property

Başlangıç hücresini alır ve ayarlar.

```csharp
public string StartCell { get; set; }
```

### Açıklamalar

Yalnızca dosya spreadsheetML olmadığında veya XML'in Excel'e eşlenmesi durumunda çalışır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyStartCellDemo
    {
        public static void Run()
        {
            // XmlLoadOptions sınıfının bir örneğini oluştur.
            XmlLoadOptions options = new XmlLoadOptions();

            // XML veri içe aktarımı için başlangıç hücresini ayarlayın
            options.StartCell = "B2";

            // Belirtilen seçenekleri kullanarak bir XML dosyasını Çalışma Kitabı'na yükle.
            Workbook workbook = new Workbook("input.xml", options);

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Özelliği göstermek için başlangıç hücresindeki değeri çıktılayın
            Console.WriteLine("Value at start cell (B2): " + worksheet.Cells["B2"].Value);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


