---
title: "ChartPoint.ArcStartPointYPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate metodunu çağırdıktan sonra pasta bölümünün başlangıç noktasının y koordinatını alır. Pasta ve Donut grafiklerine uygulanır."
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/arcstartpointypx/
---
## ChartPoint.ArcStartPointYPx property

Chart.Calculate() yöntemi çağrıldıktan sonra dilim bölümünün başlangıç noktasının y koordinatını alır. Pie ve Doughnut grafiklerine uygulanır.

```csharp
public float ArcStartPointYPx { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcStartPointYPxDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir pasta grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Şekil konumlarını elde etmek için grafiği hesaplayın
            chart.Calculate();

            // İlk grafik noktasını al
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mevcut ArcStartPointYPx değerini göster
            Console.WriteLine("Current ArcStartPointYPx value: " + point.ArcStartPointYPx);

            // Not: ArcStartPointYPx yalnızca okunabilir, bu yüzden doğrudan ayarlayamıyoruz
            // Bunun yerine, diğer özellikleri değiştirmenin ArcStartPointYPx'i nasıl etkilediğini göstereceğiz

            // Patlama değerini değiştirerek pasta diliminin konumunu değiştirin
            point.Explosion = 20;

            // Konumları güncellemek için grafiği yeniden hesaplayın
            chart.Calculate();

            // Patlamayı değiştirdikten sonra yeni ArcStartPointYPx değerini gösterin
            Console.WriteLine("New ArcStartPointYPx after explosion change: " + point.ArcStartPointYPx);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPointPropertyArcStartPointYPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


