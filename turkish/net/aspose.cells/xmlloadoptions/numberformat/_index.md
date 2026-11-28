---
title: "XmlLoadOptions.NumberFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "XmlLoadOptions özelliği. Sayısal değerin biçimini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/xmlloadoptions/numberformat/
---
## XmlLoadOptions.NumberFormat property

Sayısal değerin biçimini alır ve ayarlar.

```csharp
public string NumberFormat { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlLoadOptionsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // XmlLoadOptions sınıfının bir örneğini oluştur.
            XmlLoadOptions options = new XmlLoadOptions();

            // Sayıları 2 ondalık basamakla göstermek için NumberFormat özelliğini ayarlayın
            options.NumberFormat = "0.00";

            // Belirtilen seçenekleri kullanarak bir XML dosyasını Çalışma Kitabı'na yükle.
            Workbook workbook = new Workbook("input.xml", options);

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Sayı biçimlendirmesini göstermek için bazı sayısal değerler ayarlayın
            worksheet.Cells["A1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(45.678);
            worksheet.Cells["A3"].PutValue(0.5);

            // Çalışma kitabını yeni bir dosyaya kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


