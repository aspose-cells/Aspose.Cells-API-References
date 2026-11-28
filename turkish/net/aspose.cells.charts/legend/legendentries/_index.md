---
title: "Legend.LegendEntries"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Legend özelliği. Belirtilen grafik başlığındaki tüm LegendEntry nesnelerinin bir koleksiyonunu alır. Yüzey grafiğinin başlık girişlerini ayarlama desteklenmez. Bu nedenle grafik türü yüzey grafiği ise null dönecektir."
type: docs
url: /tr/net/aspose.cells.charts/legend/legendentries/
---
## Legend.LegendEntries property

Belirtilen grafik başlığındaki tüm LegendEntry nesnelerinin bir koleksiyonunu alır. Yüzey grafiğinin başlık girişlerini ayarlama desteklenmez. Bu nedenle grafik tipi yüzey grafiği ise null dönecektir.

```csharp
public LegendEntryCollection LegendEntries { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyLegendEntriesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // Lejant girişlerine eriş
            Aspose.Cells.Charts.LegendEntryCollection legendEntries = chart.Legend.LegendEntries;
            
            // İkinci başlık girişini sil
            legendEntries[1].IsDeleted = true;
            
            // Çalışma kitabını kaydedin
            workbook.Save("LegendEntriesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [LegendEntryCollection](../../legendentrycollection/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


