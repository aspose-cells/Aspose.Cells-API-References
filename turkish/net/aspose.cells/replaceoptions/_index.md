---
title: "ReplaceOptions sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ReplaceOptions sınıfı. Değiştirme seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/replaceoptions/
---
## ReplaceOptions class

Değiştirme seçeneklerini temsil eder.

```csharp
public class ReplaceOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ReplaceOptions](replaceoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CaseSensitive](../../aspose.cells/replaceoptions/casesensitive/) { get; set; } | Aranan dizgenin büyük/küçük harfe duyarlı olup olmadığını gösterir. |
| [FontSettings](../../aspose.cells/replaceoptions/fontsettings/) { get; set; } | Değiştirilen metin için zengin biçimlendirilmiş ayarlar. |
| [MatchEntireCellContents](../../aspose.cells/replaceoptions/matchentirecellcontents/) { get; set; } | Tüm hücre içeriklerinin eşleşip eşleşmeyeceğini gösterir |
| [RegexKey](../../aspose.cells/replaceoptions/regexkey/) { get; set; } | Aranan anahtarın regex olup olmadığını gösterir. Doğru ise aranan anahtar regex olarak alınır. |
| [StyleFlags](../../aspose.cells/replaceoptions/styleflags/) { get; set; } | Yazı tipi ayarlarının uygulanma bayraklarını alır ve ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReplaceOptionsDemo
    {
        public static void ReplaceOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı örnek veriler ekleyin
            sheet.Cells["A1"].PutValue("Hello World");
            sheet.Cells["A2"].PutValue("Hello Aspose");
            sheet.Cells["A3"].PutValue("Goodbye World");

            // ReplaceOptions oluştur
            ReplaceOptions options = new ReplaceOptions
            {
                CaseSensitive = false,
                MatchEntireCellContents = false,
                RegexKey = false
            };

            // Çalışma sayfasında "Hello" ifadesini "Hi" ile değiştir
            int replacedCount = workbook.Replace("Hello", "Hi", options);

            // Yapılan değişiklik sayısını çıktı olarak ver
            Console.WriteLine($"Number of replacements made: {replacedCount}");

            // Çalışma kitabını kaydedin
            workbook.Save("ReplaceOptionsExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


