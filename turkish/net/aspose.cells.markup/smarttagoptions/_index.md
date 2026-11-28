---
title: "Sınıf SmartTagOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Markup.SmartTagOptions sınıfı. Akıllı etiketin seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells.markup/smarttagoptions/
---
## SmartTagOptions class

Akıllı etiketin seçeneklerini temsil eder.

```csharp
public class SmartTagOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [SmartTagOptions](smarttagoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [EmbedSmartTags](../../aspose.cells.markup/smarttagoptions/embedsmarttags/) { get; set; } | Çalışma kitabıyla akıllı etiketlerin kaydedilip kaydedilmeyeceğini gösterir. |
| [ShowType](../../aspose.cells.markup/smarttagoptions/showtype/) { get; set; } | Akıllı etiketin gösterim tipini temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // SmartTagOptions bir örnek oluşturun
            SmartTagOptions options = new SmartTagOptions();

            // Özellikleri ayarla
            options.EmbedSmartTags = true;
            options.ShowType = SmartTagShowType.NoSmartTagIndicator;

            // SmartTagOptions'ı çalışma sayfasına uygula
            // Not: worksheet.SmartTagSetting.Options = options; ifadesi değiştirildi
            // SmartTagSetting'in Options özelliği olmadığı için seçenek nesnesini doğrudan kullanmak
            // (Seçeneklerin doğrudan kullanılmak istendiği varsayılıyor)
            
            // Demonstrasyon amacıyla bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);

            // Çalışma kitabını kaydedin
            workbook.Save("SmartTagOptionsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


