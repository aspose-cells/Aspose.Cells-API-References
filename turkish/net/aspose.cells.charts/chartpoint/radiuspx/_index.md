---
title: "ChartPoint.RadiusPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate metodunu çağırdıktan sonra balon pasta veya donutun yarıçapını piksel biriminde alır"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/radiuspx/
---
## ChartPoint.RadiusPx property

Chart.Calculate() metodunu çağırdıktan sonra balon, pie veya doughnut'un yarıçapını piksel biriminde alır.

```csharp
public int RadiusPx { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyRadiusPxDemo
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

            // Mevcut yarıçap değerini göster
            Console.WriteLine("Current RadiusPx value: " + point.RadiusPx);

            // Not: RadiusPx yalnızca okunabilir, bu yüzden doğrudan ayarlayamayız
            // Yarıçapı değiştirmek için grafik boyutunu veya diğer özellikleri ayarlamamız gerekir
            // bu, nokta boyutunu dolaylı olarak etkiler

            // Grafik boyutunu değiştirmenin yarıçapı nasıl etkilediğine dair örnek
            Console.WriteLine("\nChanging chart size to demonstrate radius change...");
            chart.ChartObject.Width = 800;
            chart.ChartObject.Height = 600;
            chart.Calculate();

            // Grafik yeniden boyutlandırıldıktan sonra yeni yarıçap değerini göster
            Console.WriteLine("New RadiusPx value after chart resize: " + point.RadiusPx);

            // Sonucu kaydet
            workbook.Save("ChartPointPropertyRadiusPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


