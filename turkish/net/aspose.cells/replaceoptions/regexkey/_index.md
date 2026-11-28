---
title: "ReplaceOptions.RegexKey"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ReplaceOptions özelliği. Aranan anahtarın regex olup olmadığını gösterir. Doğru ise aranan anahtar regex olarak alınır"
type: docs
url: /tr/net/aspose.cells/replaceoptions/regexkey/
---
## ReplaceOptions.RegexKey property

Aranan anahtarın regex olup olmadığını gösterir. Doğru ise aranan anahtar regex olarak alınır.

```csharp
public bool RegexKey { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyRegexKeyDemo
    {
        public static void Run()
        {
            // Örnek veriyle bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("apple");
            worksheet.Cells["A2"].PutValue("banana");
            worksheet.Cells["A3"].PutValue("orange");
            worksheet.Cells["A4"].PutValue("pear");
            worksheet.Cells["A5"].PutValue("plum");

            // Regex ile değiştirme seçenekleri oluştur
            ReplaceOptions options = new ReplaceOptions();
            options.RegexKey = true; // Enable regex matching
            
            // ‘p’ veya ‘b’ harfiyle başlayıp bir sesli harfle devam eden tüm kelimeleri değiştir
            string pattern = "^[pb][aeiou]";
            string replacement = "FRUIT";
            
            // Değiştirmeyi gerçekleştir
            workbook.Replace(pattern, replacement, options);

            // Sonucu kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


