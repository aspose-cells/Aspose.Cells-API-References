---
title: "ChartPoint.ShapeXPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. `Chart.Calculate` metodunu çağırdıktan sonra sol üst köşenin x koordinatını piksel biriminde alır"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/shapexpx/
---
## ChartPoint.ShapeXPx property

Chart.Calculate() metodunu çağırdıktan sonra sol üst köşenin x koordinatını piksel biriminde alır.

```csharp
public int ShapeXPx { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeXPxDemo
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

            // İlk seriden ilk grafik noktasını alın
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mevcut X konumunu piksel olarak göster
            Console.WriteLine("Current ShapeXPx value: " + point.ShapeXPx);

            // Not: ShapeXPx yalnızca okunabilir, bu yüzden doğrudan ayarlayamayız
            // Konumu değiştirmek için grafik boyutunu/konumunu veya verileri değiştirmemiz gerekir

            // Grafiği değiştirdiğimizde özelliğin nasıl değiştiğini göster
            Console.WriteLine("\nChanging chart position...");
            chart.ChartObject.Left = 3;
            chart.ChartObject.Top = 2;
            chart.Calculate(); // Recalculate to update positions

            Console.WriteLine("New ShapeXPx value after chart move: " + point.ShapeXPx);

            // Sonucu kaydet
            workbook.Save("ChartPointPropertyShapeXPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


