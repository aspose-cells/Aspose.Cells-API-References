---
title: "Series.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Veri serisinin adını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/series/name/
---
## Series.Name property

Veri serisinin adını alır veya ayarlar.

```csharp
public string Name { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Series Name");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].PutValue(30);
            
            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafiğe seri ekle
            chart.NSeries.Add("A2:C2", true);
            
            // Name özelliğinin kullanımını göster
            // 1. Bir hücreye referans adı
            chart.NSeries[0].Name = "=A1";
            
            // 2. İsme bir dize ayarlayın
            chart.NSeries[0].Name = "First Series";
            
            // Çalışma kitabını kaydedin
            workbook.Save("SeriesPropertyNameDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


