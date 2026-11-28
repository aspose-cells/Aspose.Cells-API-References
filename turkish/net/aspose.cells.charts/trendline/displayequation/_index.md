---
title: "Trendline.DisplayEquation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Trendline özelliği. Trend çizgi denkleminin, Rsquared değeriyle aynı veri etiketinde grafikte gösterilip gösterilmediğini temsil eder. Bu özelliği True olarak ayarlamak, veri etiketlerini otomatik olarak etkinleştirir"
type: docs
url: /tr/net/aspose.cells.charts/trendline/displayequation/
---
## Trendline.DisplayEquation property

Trend çizgisinin denkleminin grafikte (R-kare değeriyle aynı veri etiketinde) gösterilip gösterilmediğini temsil eder. Bu özelliği True olarak ayarlamak, veri etiketlerini otomatik olarak açar.

```csharp
public bool DisplayEquation { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDisplayEquationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Grafik oluştur
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Seri ve trend çizgisi ekle
            chart.NSeries.Add("A1:B4", true);
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Trend çizgisi özelliklerini yapılandır
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = false;
            trendline.Color = Color.Blue;

            workbook.Save("TrendlineDisplayEquationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


