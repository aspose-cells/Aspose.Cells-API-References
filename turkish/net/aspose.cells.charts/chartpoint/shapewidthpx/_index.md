---
title: "ChartPoint.ShapeWidthPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate metodunu çağırdıktan sonra piksel biriminde genişliği alır"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/shapewidthpx/
---
## ChartPoint.ShapeWidthPx property

Chart.Calculate() metodunu çağırdıktan sonra genişliği piksel biriminde alır.

```csharp
public int ShapeWidthPx { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeWidthPxDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
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

            // Şekil özelliklerinin kullanılabilir olmasını sağlamak için grafiği hesaplayın
            chart.Calculate();

            // İlk seriden ilk grafik noktasını al
            ChartPoint point = chart.NSeries[0].Points[0];

            // Grafik noktasının şekil genişliğini piksel cinsinden göster
            Console.WriteLine("Current ShapeWidthPx value: " + point.ShapeWidthPx);

            // Not: ShapeWidthPx yalnızca okunabilir, bu yüzden doğrudan ayarlanamaz
            // Genişliği değiştirmek için grafiğin boyutunu veya diğer özelliklerini değiştirmemiz gerekir
            // Bu, bir sonraki Calculate() sırasında noktanın genişliğini etkiler

            // Grafiğin genişliğini değiştirerek ShapeWidthPx'i nasıl etkilediğini göster
            chart.ChartObject.Width = 1000;
            chart.Calculate();

            // Grafik yeniden boyutlandırıldıktan sonra yeni genişliği göster
            Console.WriteLine("New ShapeWidthPx value after chart resize: " + point.ShapeWidthPx);

            // Sonucu kaydet
            workbook.Save("ChartPointPropertyShapeWidthPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


