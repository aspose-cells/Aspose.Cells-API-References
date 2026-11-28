---
title: "SeriesCollection.SwapSeries"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SeriesCollection yöntemi. İki serinin sırasını doğrudan değiştirir"
type: docs
url: /tr/net/aspose.cells.charts/seriescollection/swapseries/
---
## SeriesCollection.SwapSeries method

İki serinin sırasını doğrudan değiştirir.

```csharp
public void SwapSeries(int sourceIndex, int destIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceIndex | Int32 | Geçerli indeks |
| destIndex | Int32 | Hedef indeks |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodSwapSeriesWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["B4"].PutValue(15);
            
            worksheet.Cells["C1"].PutValue("Series 3");
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C3"].PutValue(16);
            worksheet.Cells["C4"].PutValue(24);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("A1:C4", true);
            
            // Seri koleksiyonunu alın
            Aspose.Cells.Charts.SeriesCollection sc = chart.NSeries;
            
            // Orijinal seri adlarını yazdır
            Console.WriteLine("Original Series Order:");
            for (int i = 0; i < sc.Count; i++)
            {
                Console.WriteLine($"Series {i}: {sc[i].Name}");
            }
            
            // Seri 0 ve 1'i değiştir
            sc.SwapSeries(0, 1);
            Console.WriteLine("\nAfter swapping series 0 and 1:");
            for (int i = 0; i < sc.Count; i++)
            {
                Console.WriteLine($"Series {i}: {sc[i].Name}");
            }
            
            // Seri 2 ve 0'ı değiştir
            sc.SwapSeries(2, 0);
            Console.WriteLine("\nAfter swapping series 2 and 0:");
            for (int i = 0; i < sc.Count; i++)
            {
                Console.WriteLine($"Series {i}: {sc[i].Name}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


