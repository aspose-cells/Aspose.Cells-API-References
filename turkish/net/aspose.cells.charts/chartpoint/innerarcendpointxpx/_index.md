---
title: "ChartPoint.InnerArcEndPointXPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate metodunu çağırdıktan sonra pasta diliminin bitiş noktasının x koordinatını alır. Doughnut grafiklerine uygulanır"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/innerarcendpointxpx/
---
## ChartPoint.InnerArcEndPointXPx property

Chart.Calculate() yöntemi çağrıldıktan sonra dilim bölümünün bitiş noktasının x koordinatını alır. Doughnut grafiklerine uygulanır.

```csharp
public float InnerArcEndPointXPx { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcEndPointXPxDemo
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
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(2);

            // Bir doughnut grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafiği hesaplayarak grafik nokta özelliklerini alın
            chart.Calculate();

            // İlk seriden ilk grafik noktasını alın
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mevcut InnerArcEndPointXPx değerini göster
            Console.WriteLine("Current InnerArcEndPointXPx value: " + point.InnerArcEndPointXPx);

            // Not: InnerArcEndPointXPx yalnızca okunur, bu yüzden doğrudan ayarlayamayız
            // Bitiş noktasının konumunu değiştirmek için doughnut deliği boyutunu değiştirmemiz gerekir
            chart.NSeries[0].DoughnutHoleSize = 50; // Set hole size to 50%

            // Özellikleri güncellemek için grafiği yeniden hesaplayın
            chart.Calculate();

            // Deliğin boyutu değiştirildikten sonra yeni InnerArcEndPointXPx değerini göster
            Console.WriteLine("New InnerArcEndPointXPx value after changing doughnut hole size: " + point.InnerArcEndPointXPx);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPointPropertyInnerArcEndPointXPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


