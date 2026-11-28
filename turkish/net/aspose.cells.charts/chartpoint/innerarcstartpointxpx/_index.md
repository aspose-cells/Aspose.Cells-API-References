---
title: "ChartPoint.InnerArcStartPointXPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate metodunu çağırdıktan sonra dilim bölümünün başlangıç noktasının x koordinatını alır. Doughnut grafiği için geçerlidir."
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/innerarcstartpointxpx/
---
## ChartPoint.InnerArcStartPointXPx property

Chart.Calculate() yöntemi çağrıldıktan sonra dilim bölümünün başlangıç noktasının x koordinatını alır. Doughnut grafiğine uygulanır.

```csharp
public float InnerArcStartPointXPx { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcStartPointXPxDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir doughnut grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Şekil özelliklerini elde etmek için grafiği hesaplayın
            chart.Calculate();

            // İlk grafik noktasını al
            ChartPoint point = chart.NSeries[0].Points[0];

            // InnerArcStartPointXPx değerini göster
            Console.WriteLine("InnerArcStartPointXPx: " + point.InnerArcStartPointXPx);

            // Not: InnerArcStartPointXPx yalnızca okunabilir, bu yüzden doğrudan ayarlayamıyoruz
            // Pozisyonu değiştirmek için grafik boyutunu veya doughnut delik boyutunu değiştirmemiz gerekir

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPointPropertyInnerArcStartPointXPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


