---
title: "Enum OoxmlCompressionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.OoxmlCompressionType enum. Ooxml sıkıştırma türü"
type: docs
url: /tr/net/aspose.cells/ooxmlcompressiontype/
---
## OoxmlCompressionType enumeration

OOXML sıkıştırma türü

```csharp
public enum OoxmlCompressionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Level1 | `1` | En hızlı ancak en az etkili sıkıştırma. |
| Level2 | `2` | Seviye 1'den biraz daha yavaş, ama daha iyi. |
| Level3 | `3` | Seviye 2'den biraz daha yavaş, ama daha iyi. |
| Level4 | `4` | Seviye 3'den biraz daha yavaş, ama daha iyi. |
| Level5 | `5` | Seviye 4'ten biraz daha yavaş, ancak daha iyi sıkıştırma ile. |
| Level6 | `6` | Hız ve sıkıştırma verimliliği arasında iyi bir denge. |
| Level7 | `7` | Oldukça iyi sıkıştırma! |
| Level8 | `8` | Level7'ye göre daha iyi sıkıştırma! |
| Level9 | `9` | "en iyi" sıkıştırma, burada en iyi, giriş veri akışının boyutundaki en büyük azalmayı ifade eder. Bu aynı zamanda en yavaş sıkıştırmadır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlCompressionTypeDemo
    {
        public static void OoxmlCompressionTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // OoxmlSaveOptions oluştur ve sıkıştırma türünü ayarla
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6; // A good balance of speed and compression efficiency

            // Belirtilen sıkıştırma türüyle çalışma kitabını kaydet
            workbook.Save("OoxmlCompressionTypeExample.xlsx", saveOptions);

            Console.WriteLine("Workbook saved with OoxmlCompressionType.Level6 compression.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


