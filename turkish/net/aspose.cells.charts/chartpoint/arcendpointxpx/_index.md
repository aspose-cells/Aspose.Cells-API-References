---
title: "ChartPoint.ArcEndPointXPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate metodunu çağırdıktan sonra pasta diliminin bitiş noktasının x koordinatını alır. Pie ve Doughnut grafiklerine uygulanır"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/arcendpointxpx/
---
## ChartPoint.ArcEndPointXPx property

Chart.Calculate() yöntemi çağrıldıktan sonra dilim bölümünün bitiş noktasının x koordinatını alır. Pie ve Doughnut grafiklerine uygulanır.

```csharp
public float ArcEndPointXPx { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcEndPointXPxDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Bir pasta grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafiği hesaplayarak özelliklerin doldurulmasını sağlayın
            chart.Calculate();

            // İlk grafik noktasını al
            ChartPoint point = chart.NSeries[0].Points[0];

            // ArcEndPointXPx değerini göster
            Console.WriteLine("ArcEndPointXPx: " + point.ArcEndPointXPx);

            // Not: ArcEndPointXPx yalnızca okunur, bu yüzden doğrudan ayarlayamayız
            // Bitiş noktasını değiştirmek için grafik verilerini veya pasta dilimini etkileyen özellikleri değiştirmemiz gerekir
            
            // Veri değiştirmenin ArcEndPointXPx'i nasıl etkilediğine dair örnek
            worksheet.Cells["B2"].PutValue(60); // Increase Apple's value
            chart.Calculate(); // Recalculate chart

            // Veri değişikliğinden sonra yeni ArcEndPointXPx değerini göster
            Console.WriteLine("New ArcEndPointXPx after data change: " + point.ArcEndPointXPx);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPointPropertyArcEndPointXPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


