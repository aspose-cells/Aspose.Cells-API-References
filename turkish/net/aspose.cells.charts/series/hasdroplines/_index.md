---
title: "Series.HasDropLines"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Series özelliği. Grafik düşey çizgilere sahipse True. Yalnızca çizgi grafiği veya alan grafiklerinde uygulanır"
type: docs
url: /tr/net/aspose.cells.charts/series/hasdroplines/
---
## Series.HasDropLines property

Grafiğin düşen çizgilere sahip olması durumunda doğrudur. Yalnızca satır grafiği veya alan grafiklerinde uygulanır.

```csharp
public bool HasDropLines { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasDropLinesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir çizgi grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Seri verisi ekle
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk seriyi al
            Series series = chart.NSeries[0];

            // HasDropLines özelliğini göster
            series.HasDropLines = true; // Enable drop lines
            series.Type = ChartType.Line; // Ensure it's a line chart for drop lines to be visible

            // Çalışma kitabını kaydedin
            workbook.Save("SeriesHasDropLinesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


