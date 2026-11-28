---
title: "Series.BubbleSizes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Grafik serisinin balon boyutu değerlerini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/series/bubblesizes/
---
## Series.BubbleSizes property

Grafik serisinin balon boyutu değerlerini alır veya ayarlar.

```csharp
public string BubbleSizes { get; set; }
```

### Açıklamalar

Yalnızca Bubble veya Bubble3D için.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBubbleSizesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Balon grafiği için örnek veri ekle
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            worksheet.Cells["C1"].PutValue("Bubble Sizes");
            
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
                worksheet.Cells["C" + i].PutValue(i * 0.5);
            }

            // Bir balon grafiği ekle
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Bubble, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // BubbleSizes özelliğini kullanarak seri verilerini ayarlayın
            chart.NSeries.Add("A2:A5", true);
            chart.NSeries[0].XValues = "B2:B5";
            chart.NSeries[0].BubbleSizes = "C2:C5";

            // Çalışma kitabını kaydedin
            workbook.Save("BubbleChartDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


