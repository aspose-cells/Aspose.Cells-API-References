---
title: "Series.Smooth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Seri özelliği. Eğri yumuşatmayı temsil eder. Çizgi grafiği veya dağılım grafiği için eğri yumuşatma etkinse doğru. Yalnızca çizgi grafiklerine ve çizgili dağılım grafiklerine uygulanır"
type: docs
url: /tr/net/aspose.cells.charts/series/smooth/
---
## Series.Smooth property

Eğri yumuşatmayı temsil eder. Çizgi grafiği veya dağılım grafiği için eğri yumuşatma etkinse doğru. Yalnızca çizgi grafikleri ve çizgili dağılım grafiklerine uygulanır.

```csharp
public bool Smooth { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySmoothDemo
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

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk seri için Smooth özelliğini ayarlayın
            chart.NSeries[0].Smooth = true;

            // Çalışma kitabını kaydedin
            workbook.Save("SmoothPropertyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


