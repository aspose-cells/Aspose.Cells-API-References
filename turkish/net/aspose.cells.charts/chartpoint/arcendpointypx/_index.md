---
title: "ChartPoint.ArcEndPointYPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate yöntemi çağrıldıktan sonra pasta diliminin bitiş noktasının y koordinatını alır. Pie ve Doughnut grafiklerine uygulanır"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/arcendpointypx/
---
## ChartPoint.ArcEndPointYPx property

Chart.Calculate() yöntemi çağrıldıktan sonra dilim bölümünün bitiş noktasının y koordinatını alır. Pie ve Doughnut grafiklerine uygulanır.

```csharp
public float ArcEndPointYPx { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyArcEndPointYPxDemo
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
            worksheet.Cells["B2"].PutValue(8000);
            worksheet.Cells["B3"].PutValue(12000);
            worksheet.Cells["B4"].PutValue(14000);

            // Bir pasta grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Şekil konumlarını elde etmek için grafiği hesaplayın
            chart.Calculate();

            // İlk grafik noktasını al
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mevcut ArcEndPointYPx değerini göster
            Console.WriteLine("Current ArcEndPointYPx value: " + point.ArcEndPointYPx);

            // ArcEndPointYPx yalnızca okunabilir olduğundan, sadece okuyabiliriz
            // Aşağıdaki satır bir derleme hatasına neden olur:
            // point.ArcEndPointYPx = 150.5f;

            // Bu özelliğin pasta grafiğini nasıl etkilediğini gösterin
            Console.WriteLine("Pie slice end point Y coordinate: " + point.ArcEndPointYPx + " pixels");

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPointPropertyArcEndPointYPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


