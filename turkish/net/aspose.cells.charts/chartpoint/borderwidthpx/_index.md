---
title: "ChartPoint.BorderWidthPx"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPoint özelliği. Chart.Calculate yöntemi çağrıldıktan sonra kenarlığın genişliğini piksel biriminde alır"
type: docs
url: /tr/net/aspose.cells.charts/chartpoint/borderwidthpx/
---
## ChartPoint.BorderWidthPx property

Chart.Calculate() yöntemi çağrıldıktan sonra kenarlığın piksel birimindeki genişliğini alır.

```csharp
public int BorderWidthPx { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ChartPointPropertyBorderWidthPxDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);
            worksheet.Cells["B5"].PutValue(2100);

            // Bir grafik ekleyin ve veri aralığını ayarlayın
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Özelliklerin doldurulduğundan emin olmak için grafiği hesapla
            chart.Calculate();

            // İlk serideki ilk grafik noktasını al
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mevcut kenarlık genişliğini göster
            Console.WriteLine("Current BorderWidthPx value: " + point.BorderWidthPx);

            // Not: BorderWidthPx yalnızca okunabilir, bu yüzden doğrudan ayarlayamıyoruz
            // Bunun yerine, kenarlığı Border özelliği aracılığıyla değiştirebiliriz
            if (point.Border != null)
            {
                // WeightType enum'ını kullanarak ağırlığı ayarlayarak kenarlık genişliğini değiştirin
                point.Border.Weight = WeightType.MediumLine; // Medium weight border
            }

            // BorderWidthPx değerini güncellemek için yeniden hesaplayın
            chart.Calculate();

            // Yeni kenarlık genişliğini piksel olarak göster
            Console.WriteLine("New BorderWidthPx value after modification: " + point.BorderWidthPx);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPointPropertyBorderWidthPxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


