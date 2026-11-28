---
title: "ChartPoint.ShapeHeight"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate yöntemi çağrıldıktan sonra grafiğin yüksekliğinin 1/4000 biriminde yüksekliği alır"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/shapeheight/
---
## ChartPoint.ShapeHeight property

Chart.Calculate() metodunu çağırdıktan sonra grafiğin yüksekliğinin 1/4000 biriminde yüksekliği alır.

```csharp
public int ShapeHeight { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeHeightDemo
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
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Şekil özelliklerinin kullanılabilir olmasını sağlamak için grafiği hesaplayın
            chart.Calculate();

            // İlk serideki ilk noktayı alın
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mevcut ShapeHeight değerini göster (grafiğin yüksekliğinin 1/4000 biriminde)
            Console.WriteLine("Current ShapeHeight value: " + point.ShapeHeight);

            // Not: ShapeHeight yalnızca okunabilir, bu yüzden doğrudan ayarlayamayız
            // Yüksekliği değiştirmek için grafiğin boyutunu veya diğer özellikleri değiştirmemiz gerekir

            // Grafik yüksekliğini değiştirerek etkiyi gösterin
            Console.WriteLine("Original chart height: " + chart.ChartObject.Height);
            chart.ChartObject.Height = 400;
            chart.Calculate(); // Recalculate to update shape properties

            // Grafik yüksekliği değiştirildikten sonra yeni ShapeHeight değerini göster
            Console.WriteLine("New ShapeHeight value after chart resize: " + point.ShapeHeight);

            // Sonucu kaydet
            workbook.Save("ChartPointPropertyShapeHeightDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


