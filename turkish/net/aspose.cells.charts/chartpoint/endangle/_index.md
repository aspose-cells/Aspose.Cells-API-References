---
title: "ChartPoint.EndAngle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate metodunu çağırdıktan sonra x ekseninden saat yönünde derece cinsinden ölçülen pasta bölümünün bitiş açısını alır. Pasta grafiğine uygulanır."
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/endangle/
---
## ChartPoint.EndAngle property

Chart.Calculate() yöntemi çağrıldıktan sonra x ekseninden saat yönünde derece cinsinden ölçülen dilim bölümünün bitiş açısını alır. Pie grafiğine uygulanır.

```csharp
public float EndAngle { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyEndAngleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pasta grafiği için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Bir pasta grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafiği hesaplayarak özelliklerin doldurulmasını sağlayın
            chart.Calculate();

            // İlk grafik noktasını al (Elma dilimi)
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mevcut EndAngle değerini göster
            Console.WriteLine("Current EndAngle value: " + point.EndAngle);

            // Not: EndAngle yalnızca okunabilir, bu yüzden doğrudan ayarlanamaz
            // Bunun yerine, bunun pasta dilimiyle nasıl ilişkili olduğunu göstereceğiz

            // Noktayı patlatarak açıların nasıl etkilendiğini gör
            point.Explosion = 20;
            chart.Calculate(); // Recalculate to update angles

            // Patlamadan sonra yeni EndAngle değerini göster
            Console.WriteLine("EndAngle after explosion: " + point.EndAngle);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPointEndAngleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


