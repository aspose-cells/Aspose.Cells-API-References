---
title: "Sınıf Top10Filter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Top10Filter sınıfı. Filtrelenecek en üst N yüzde ya da öğe sayısını temsil eder"
type: docs
url: /tr/net/aspose.cells/top10filter/
---
## Top10Filter class

Filtrelenecek en üst N'i (yüzde ya da öğe sayısı) temsil eder.

```csharp
public class Top10Filter
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Criteria](../../aspose.cells/top10filter/criteria/) { get; set; } | (**Obsolete.**) Bu filtre için karşılaştırma yapmak üzere kullanılan aralıktaki gerçek hücre değeri. Bu, yenileme işlemi sırasında önbellek değeridir. |
| [IsPercent](../../aspose.cells/top10filter/ispercent/) { get; set; } | Sütunun yüzde değeriyle filtreleme yapılıp yapılmayacağını gösterir. |
| [IsTop](../../aspose.cells/top10filter/istop/) { get; set; } | Üst sıraya göre filtreleme yapılıp yapılmayacağını gösterir. |
| [Items](../../aspose.cells/top10filter/items/) { get; set; } | Filtre kriteri olarak kullanılacak üst veya alt değeri alır ve ayarlar. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTop10FilterDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["B6"].PutValue("Value");
            for (int i = 7; i <= 16; i++)
            {
                worksheet.Cells["B" + i].PutValue(20 - i);
                worksheet.Cells["C" + i].PutValue("Item " + (i-6));
            }
            
            // Otomatik filtreyi ve ilk 10 filtresini uygulayın.
            worksheet.AutoFilter.Range = "B6:C16";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5); // Filter top 5 values in column B
            
            // Top10Filter'ı alın ve özelliklerini doğrulayın.
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop);
            Console.WriteLine("IsPercent: " + filter.IsPercent);
            Console.WriteLine("Items: " + filter.Items);
            
            // Filtreyi yenileyin ve gizli satırları kontrol edin.
            worksheet.AutoFilter.Refresh();
            for (int i = 6; i <= 16; i++)
            {
                Console.WriteLine($"Row {i} hidden: {worksheet.Cells.IsRowHidden(i)}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("Top10FilterDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


