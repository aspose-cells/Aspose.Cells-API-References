---
title: "Top10Filter.IsPercent"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Top10Filter özelliği. Sütunun yüzde değerine göre filtreleyip filtrelemeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/top10filter/ispercent/
---
## Top10Filter.IsPercent property

Sütunun yüzde değeriyle filtreleme yapılıp yapılmayacağını gösterir.

```csharp
public bool IsPercent { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyIsPercentDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue((i + 1) * (j + 1));
                }
            }

            // Üst 10 filtresini uygula (yüzde değil)
            worksheet.AutoFilter.Range = "A1:J10";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // Filtreyi al ve IsPercent özelliğini göster
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop);
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output False

            // Üst 10 yüzde filtresini uygula
            worksheet.AutoFilter.FilterTop10(1, true, true, 20);
            filter = worksheet.AutoFilter.FilterColumns[1].Filter as Top10Filter;
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output True
        }
    }
}
```

### Ayrıca Bakınız

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


