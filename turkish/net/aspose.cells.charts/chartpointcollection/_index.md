---
title: "Sınıf ChartPointCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.ChartPointCollection sınıfı. Bir serideki tüm noktaları içeren bir koleksiyonu temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/chartpointcollection/
---
## ChartPointCollection class

Bir serideki tüm noktaları içeren bir koleksiyonu temsil eder.

```csharp
public class ChartPointCollection : IEnumerable
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.cells.charts/chartpointcollection/count/) { get; } | Grafik noktasının sayısını alır. |
| [Item](../../aspose.cells.charts/chartpointcollection/item/) { get; } | Seride belirtilen indeksteki [`ChartPoint`](../chartpoint/) öğesini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Clear](../../aspose.cells.charts/chartpointcollection/clear/)() | Grafik noktalarının tüm ayarlarını kaldır. |
| [GetEnumerator](../../aspose.cells.charts/chartpointcollection/getenumerator/)() | Tüm `ChartPointCollection` için bir yineleyici döndürür. |
| [RemoveAt](../../aspose.cells.charts/chartpointcollection/removeat/)(int) | Serinin indeksindeki noktayı kaldırır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointCollectionDemo
    {
        public static void ChartPointCollectionExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasının referansını elde etme
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere örnek değerler ekleme
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Çalışma sayfasına bir grafik ekleme
            int chartIndex = worksheet.Charts.Add(ChartType.PieExploded, 5, 0, 25, 10);

            // Yeni eklenen grafiğin örneğine erişme
            Chart chart = worksheet.Charts[chartIndex];

            // Grafiğe, "A1" hücresinden "B3" hücresine kadar uzanan NSeries (grafik veri kaynağı) ekleniyor
            chart.NSeries.Add("A1:B3", true);

            // Veri Etiketlerini Göster 
            chart.NSeries[0].DataLabels.ShowValue = true;

            // ChartPointCollection'a erişim
            ChartPointCollection points = chart.NSeries[0].Points;

            // Koleksiyondaki noktalar arasında yineleme
            for (int i = 0; i < points.Count; i++)
            {
                // Veri Noktasını Al
                ChartPoint point = points[i];
                
                // Pasta Patlamasını Ayarla
                point.Explosion = 15;
                
                // Kenarlık Rengini Ayarla
                point.Border.Color = System.Drawing.Color.Red;
            }

            // Excel dosyasını kaydetme
            workbook.Save("ChartPointCollectionExample.xlsx");
            workbook.Save("ChartPointCollectionExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


