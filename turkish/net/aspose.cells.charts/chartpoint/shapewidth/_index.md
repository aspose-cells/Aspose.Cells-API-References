---
title: "ChartPoint.ShapeWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate metodunu çağırdıktan sonra grafiğin genişliğinin 1/4000 biriminde genişliği alır."
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/shapewidth/
---
## ChartPoint.ShapeWidth property

Chart.Calculate() metodunu çağırdıktan sonra grafiğin genişliğinin 1/4000 biriminde genişliği alır.

```csharp
public int ShapeWidth { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyShapeWidthDemo
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
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Şekil özelliklerinin kullanılabilir olmasını sağlamak için grafiği hesaplayın
            chart.Calculate();
            
            // İlk serideki ilk grafik noktasını al
            ChartPoint point = chart.NSeries[0].Points[0];
            
            // Mevcut ShapeWidth değerini göster (grafiğin genişliğinin 1/4000 biriminde).
            Console.WriteLine("Current ShapeWidth value: " + point.ShapeWidth);
            
            // Genişliği piksel cinsinden göster.
            Console.WriteLine("Shape width in pixels: " + point.ShapeWidthPx);
            
            // Not: ShapeWidth sadece okunabilir, bu yüzden doğrudan ayarlanamaz.
            // Genişliği değiştirmek için grafiğin boyutunu veya diğer özellikleri değiştirmemiz gerekir.
            
            // Sonucu kaydet
            workbook.Save("ChartPointShapeWidthDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


