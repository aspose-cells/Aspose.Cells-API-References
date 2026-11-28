---
title: "Trendline.Intercept"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Trendline özelliği. Trend çizgisinin değer eksenini kestiği noktayı döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/trendline/intercept/
---
## Trendline.Intercept property

Trend çizgisinin değer eksenini kestiği noktayı döndürür veya ayarlar.

```csharp
public double Intercept { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyInterceptDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(6);

            // Grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Trend çizgisi ekle ve kesişim noktasını ayarla
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Intercept = 1.0; // Setting the Y-intercept value
            trendline.DisplayEquation = true;

            workbook.Save("TrendlineInterceptDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


