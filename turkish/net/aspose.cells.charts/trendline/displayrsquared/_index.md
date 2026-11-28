---
title: "Trendline.DisplayRSquared"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Trendline özelliği. Trend çizgisinin Rsquared değerinin denkleme aynı veri etiketi içinde grafikte gösterilip gösterilmediğini belirtir. Bu özelliği True olarak ayarlamak, veri etiketlerini otomatik olarak etkinleştirir."
type: docs
url: /tr/net/aspose.cells.charts/trendline/displayrsquared/
---
## Trendline.DisplayRSquared property

Trend çizgisinin R-kare değerinin grafikte (denklemle aynı veri etiketi içinde) gösterilip gösterilmediğini temsil eder. Bu özelliği True olarak ayarlamak, veri etiketlerini otomatik olarak açar.

```csharp
public bool DisplayRSquared { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDisplayRSquaredDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(4);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(6);
            worksheet.Cells["B4"].PutValue(8);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // Bir trend çizgisi ekleyin ve indeksle alın
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            
            // DisplayRSquared özelliğini göster
            trendline.DisplayRSquared = true;
            trendline.DisplayEquation = true;

            // Çalışma kitabını kaydedin
            workbook.Save("TrendlineDisplayRSquaredDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


