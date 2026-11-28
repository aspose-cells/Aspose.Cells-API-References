---
title: "ChartPoint.InnerArcEndPointYPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate metodunu çağırdıktan sonra pasta diliminin bitiş noktasının y koordinatını alır. Donut grafiği için geçerlidir"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/innerarcendpointypx/
---
## ChartPoint.InnerArcEndPointYPx property

Chart.Calculate() yöntemi çağrıldıktan sonra dilim bölümünün bitiş noktasının y koordinatını alır. Doughnut grafiğine uygulanır.

```csharp
public float InnerArcEndPointYPx { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcEndPointYPxDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("C1");
            worksheet.Cells["A3"].PutValue("C2");
            worksheet.Cells["A4"].PutValue("C3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["B3"].PutValue(35);
            worksheet.Cells["B4"].PutValue(25);

            // Bir doughnut grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafiği hesaplayarak grafik nokta özelliklerini alın
            chart.Calculate();

            // İlk seriden ilk grafik noktasını alın
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mevcut InnerArcEndPointYPx değerini göster
            Console.WriteLine("Current InnerArcEndPointYPx value: " + point.InnerArcEndPointYPx);

            // Not: InnerArcEndPointYPx yalnızca okunabilir, bu yüzden doğrudan ayarlayamayız
            // Pozisyonu değiştirmek için donut deliği boyutunu değiştirmemiz gerekir
            chart.NSeries[0].DoughnutHoleSize = 60; // Change hole size to affect inner arc position

            // Özellikleri güncellemek için grafiği yeniden hesaplayın
            chart.Calculate();

            // Delik boyutu değiştirildikten sonra yeni InnerArcEndPointYPx değerini göster
            Console.WriteLine("New InnerArcEndPointYPx value after changing hole size: " + point.InnerArcEndPointYPx);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPointPropertyInnerArcEndPointYPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


