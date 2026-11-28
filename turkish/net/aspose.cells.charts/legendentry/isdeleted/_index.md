---
title: "LegendEntry.IsDeleted"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LegendEntry özelliği. Lejant girişinin silinip silinmediğini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/legendentry/isdeleted/
---
## LegendEntry.IsDeleted property

Legend girişinin silinip silinmediğini alır ve ayarlar.

```csharp
public bool IsDeleted { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // İlk lejant girişini al
            LegendEntry legendEntry = chart.Legend.LegendEntries[0];

            // IsDeleted özelliğini göster
            Console.WriteLine("Legend entry initially deleted? " + legendEntry.IsDeleted);
            
            // Lejant girişini sil
            legendEntry.IsDeleted = true;
            Console.WriteLine("Legend entry after deletion? " + legendEntry.IsDeleted);

            // Lejant girişini geri yükle
            legendEntry.IsDeleted = false;
            Console.WriteLine("Legend entry after restoration? " + legendEntry.IsDeleted);

            // Çalışma kitabını kaydedin
            workbook.Save("LegendEntryIsDeletedDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


