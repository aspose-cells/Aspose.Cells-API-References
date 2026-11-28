---
title: "Trendline.DataLabels"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Trendline özelliği. Belirtilen seri için DataLabels nesnesini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/trendline/datalabels/
---
## Trendline.DataLabels property

Belirtilen seri için DataLabels nesnesini temsil eder.

```csharp
public DataLabels DataLabels { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDataLabelsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("X Values");
            sheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
            }

            // Grafik oluştur
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Seri ekle ve trend çizgisini ayarla
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries[0].XValues = "A2:A10";
            chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "Linear Trend");

            // Trend çizgisi için DataLabels'ı yapılandır
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            trendline.DataLabels.ShowValue = true;
            trendline.DataLabels.Font.Color = Color.Red;
            trendline.DataLabels.Font.IsBold = true;
            trendline.DataLabels.Position = LabelPositionType.Above;
            trendline.DataLabels.Border.IsVisible = true;
            trendline.DataLabels.Border.Color = Color.Black;

            // Çalışma kitabını kaydedin
            workbook.Save("TrendlineDataLabelsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DataLabels](../../datalabels/)
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


