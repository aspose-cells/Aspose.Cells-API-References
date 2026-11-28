---
title: "ChartPoint.ShapeY"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate yöntemi çağrıldıktan sonra grafiğin yüksekliğinin 1/4000 biriminde sol üst köşenin y koordinatını alır."
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/shapey/
---
## ChartPoint.ShapeY property

Chart.Calculate() metodunu çağırdıktan sonra grafiğin yüksekliğinin 1/4000 biriminde sol üst köşenin y koordinatını alır.

```csharp
public int ShapeY { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeYDemo
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

            // Bir sütun grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Şekil konumlarını elde etmek için grafiği hesapla
            chart.Calculate();

            // İlk serideki ilk noktayı alın
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mevcut ShapeY değerini (grafiğin yüksekliğinin 1/4000'i) göster.
            Console.WriteLine("Current ShapeY value: " + point.ShapeY);

            // Not: ShapeY yalnızca okunabilir, bu yüzden doğrudan ayarlayamıyoruz.
            // Pozisyonu değiştirmek için temel verileri veya grafik özelliklerini değiştirmemiz gerekir.

            // ShapeY'nin gerçek konumla nasıl ilişkili olduğunu gösterin.
            Console.WriteLine("ShapeY in pixels: " + point.ShapeYPx);
            Console.WriteLine("Chart height in pixels: " + (point.ShapeYPx * 4000 / point.ShapeY));

            // Sonucu kaydet
            workbook.Save("ChartPointPropertyShapeYDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


