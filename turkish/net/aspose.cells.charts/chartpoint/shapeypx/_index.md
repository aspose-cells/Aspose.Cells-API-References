---
title: "ChartPoint.ShapeYPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate yöntemi çağrıldıktan sonra sol üst köşenin y koordinatını piksel biriminde alır"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/shapeypx/
---
## ChartPoint.ShapeYPx property

Chart.Calculate() metodunu çağırdıktan sonra sol üst köşenin y koordinatını piksel biriminde alır.

```csharp
public int ShapeYPx { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeYPxDemo
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

            // Şekil konumlarını elde etmek için grafiği hesapla
            chart.Calculate();

            // İlk serideki ilk noktayı al
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mevcut Y konumunu piksel olarak göster
            Console.WriteLine("Current ShapeYPx value: " + point.ShapeYPx);

            // Not: ShapeYPx yalnızca okunabilir, bu yüzden doğrudan ayarlayamayız
            // Konumu değiştirmek için grafik boyutunu/konumunu veya verileri değiştirmemiz gerekir

            // Grafik konumunu değiştirerek nokta konumlarını etkileyen etkiyi göster
            chart.Move(2, 3, 17, 11); // Move chart to row 2, column 3
            chart.Calculate(); // Recalculate to update positions

            // Grafik hareket ettirildikten sonra yeni Y konumunu göster
            Console.WriteLine("New ShapeYPx value after chart movement: " + point.ShapeYPx);

            // Sonucu kaydet
            workbook.Save("ChartPointShapeYPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


