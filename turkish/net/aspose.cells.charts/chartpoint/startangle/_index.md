---
title: "ChartPoint.StartAngle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. `Chart.Calculate` metodunu çağırdıktan sonra x ekseninden saat yönünde derece cinsinden ölçülen pasta diliminin başlangıç açısını alır. Pasta grafiği için geçerlidir"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/startangle/
---
## ChartPoint.StartAngle property

Chart.Calculate() metodunu çağırdıktan sonra x ekseninden saat yönünde derece cinsinden ölçülen pie diliminin başlangıç açısını alır. Pie grafiği için geçerlidir.

```csharp
public float StartAngle { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyStartAngleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
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
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafiği hesaplayarak özelliklerin doldurulmasını sağlayın
            chart.Calculate();

            // İlk grafik noktasını al
            ChartPoint point = chart.NSeries[0].Points[0];

            // StartAngle değerini göster
            Console.WriteLine("StartAngle of first pie slice: " + point.StartAngle);

            // Not: StartAngle yalnızca okunabilir, bu yüzden doğrudan ayarlayamayız
            // Başlangıç açısını değiştirmek için tüm pasta grafiğini döndürmemiz gerekir
            chart.NSeries[0].FirstSliceAngle = 90; // Rotate pie chart by 90 degrees

            // Açıları güncellemek için yeniden hesapla
            chart.Calculate();

            // Döndürmeden sonra yeni StartAngle değerini göster
            Console.WriteLine("StartAngle after rotation: " + point.StartAngle);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPointPropertyStartAngleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


