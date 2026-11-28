---
title: "Series.BubbleScale"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Belirtilen grafik grubundaki balonlar için ölçek faktörünü alır veya ayarlar. Varsayılan boyutun yüzde karşılığı olarak 0'dan 300'e kadar bir tam sayı değeri olabilir. Yalnızca balon grafiklerinde uygulanır"
type: docs
url: /tr/net/aspose.cells.charts/series/bubblescale/
---
## Series.BubbleScale property

Belirtilen grafik grubundaki balonlar için ölçek faktörünü alır veya ayarlar. 0 (sıfır) ile 300 arasında bir tam sayı değer olabilir ve varsayılan boyutun yüzdesine karşılık gelir. Yalnızca balon grafiklerinde uygulanır.

```csharp
public int BubbleScale { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBubbleScaleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Balon grafiği için örnek veri ekle
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["C1"].PutValue("Size");
            
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C2"].PutValue(5);
            
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["C3"].PutValue(10);
            
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C4"].PutValue(15);

            // Bir balon grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafiğe seri ekle
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries[seriesIndex].XValues = "A2:A4";
            chart.NSeries[seriesIndex].BubbleSizes = "C2:C4";
            
            // Özelliği göstermek için balon ölçeğini ayarlayın
            chart.NSeries[seriesIndex].BubbleScale = 150; // Scale bubbles to 150% of default size
            
            // Grafik görünümünü özelleştir
            chart.Title.Text = "Bubble Chart with Scaled Bubbles";
            chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.LightBlue, 0.5, Aspose.Cells.Drawing.GradientStyleType.Horizontal, 1);
            
            // Çalışma kitabını kaydedin
            workbook.Save("BubbleScaleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


