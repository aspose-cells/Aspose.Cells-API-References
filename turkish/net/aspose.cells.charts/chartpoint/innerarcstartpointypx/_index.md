---
title: "ChartPoint.InnerArcStartPointYPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate metodunu çağırdıktan sonra pasta diliminin başlangıç noktasının y koordinatını alır. Donut grafiği için geçerlidir"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/innerarcstartpointypx/
---
## ChartPoint.InnerArcStartPointYPx property

Chart.Calculate() metodunu çağırdıktan sonra dilim bölümünün başlangıç noktasının y koordinatını alır. Doughnut grafiği için geçerlidir.

```csharp
public float InnerArcStartPointYPx { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcStartPointYPxDemo
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
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafiği hesaplayarak özelliklerin doldurulmasını sağlayın
            chart.Calculate();

            // İlk grafik noktasını al
            ChartPoint point = chart.NSeries[0].Points[0];

            // InnerArcStartPointYPx değerini göster
            Console.WriteLine("InnerArcStartPointYPx: " + point.InnerArcStartPointYPx);

            // Not: InnerArcStartPointYPx yalnızca okunabilir, bu yüzden doğrudan ayarlayamayız
            // Pozisyonu değiştirmek için donut deliği boyutunu ayarlamamız gerekir
            chart.NSeries[0].DoughnutHoleSize = 50; // Percentage of the chart size

            // Özellikleri güncellemek için grafiği yeniden hesaplayın
            chart.Calculate();

            // Delik boyutu değiştirildikten sonra yeni InnerArcStartPointYPx değerini göster
            Console.WriteLine("New InnerArcStartPointYPx after changing hole size: " + point.InnerArcStartPointYPx);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPointPropertyInnerArcStartPointYPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


