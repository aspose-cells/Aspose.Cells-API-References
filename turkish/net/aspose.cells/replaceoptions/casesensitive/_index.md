---
title: "ReplaceOptions.CaseSensitive"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ReplaceOptions özelliği. Aranan dizgenin büyük/küçük harfe duyarlı olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/replaceoptions/casesensitive/
---
## ReplaceOptions.CaseSensitive property

Aranan dizgenin büyük/küçük harfe duyarlı olup olmadığını gösterir.

```csharp
public bool CaseSensitive { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyCaseSensitiveDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veriyi ayarla
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("APPLE");

            // CaseSensitive = false ile değiştirme seçenekleri oluştur
            ReplaceOptions options = new ReplaceOptions();
            options.CaseSensitive = false;
            
            // "apple" kelimesinin tüm büyük/küçük harf varyasyonlarını "orange" ile değiştir
            workbook.Replace("apple", "orange", options);

            // Sonuçları çıktı olarak ver
            Console.WriteLine("After replacement (CaseSensitive = false):");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }

            // Verileri sıfırla
            worksheet.Cells["A2"].PutValue("apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("APPLE");

            // CaseSensitive = true olarak değiştir
            options.CaseSensitive = true;
            workbook.Replace("apple", "orange", options);

            // Sonuçları çıktı olarak ver
            Console.WriteLine("\nAfter replacement (CaseSensitive = true):");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


