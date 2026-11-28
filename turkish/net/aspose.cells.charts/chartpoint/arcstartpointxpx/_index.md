---
title: "ChartPoint.ArcStartPointXPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate metodunu çağırdıktan sonra dilim bölümünün başlangıç noktasının x koordinatını alır. Pasta ve Donut grafiklerine uygulanır."
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/arcstartpointxpx/
---
## ChartPoint.ArcStartPointXPx property

Chart.Calculate() yöntemi çağrıldıktan sonra dilim bölümünün başlangıç noktasının x koordinatını alır. Pie ve Doughnut grafiklerine uygulanır.

```csharp
public float ArcStartPointXPx { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcStartPointXPxDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir pasta grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafiği hesaplayarak özelliklerin doldurulmasını sağlayın
            chart.Calculate();

            // İlk grafik noktasını al
            ChartPoint point = chart.NSeries[0].Points[0];

            // ArcStartPointXPx değerini göster
            Console.WriteLine("ArcStartPointXPx for first point: " + point.ArcStartPointXPx);

            // Not: ArcStartPointXPx yalnızca okunabilir, bu yüzden doğrudan ayarlanamaz
            // Bunun yerine, diğer özellikleri değiştirdiğimizde nasıl değiştiğini gösterebiliriz

            // Pasta dilimi konumunu etkileyen patlama değerini değiştir
            point.Explosion = 20;
            chart.Calculate(); // Recalculate to update properties

            // Patlama değişikliğinden sonra yeni ArcStartPointXPx değerini göster
            Console.WriteLine("ArcStartPointXPx after explosion: " + point.ArcStartPointXPx);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPointPropertyArcStartPointXPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


