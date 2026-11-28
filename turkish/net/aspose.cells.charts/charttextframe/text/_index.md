---
title: "ChartTextFrame.Text"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartTextFrame özelliği. Çerçevenin başlığının metnini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/charttextframe/text/
---
## ChartTextFrame.Text property

Bir çerçevenin başlığının metnini alır veya ayarlar.

```csharp
public virtual string Text { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["A2"].PutValue("A");
            cells["A3"].PutValue("B");
            cells["A4"].PutValue("C");
            cells["B1"].PutValue("Value");
            cells["B2"].PutValue(10);
            cells["B3"].PutValue(20);
            cells["B4"].PutValue(30);

            // Grafik ekle
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Grafik başlığı metnini ayarla
            chart.Title.Text = "Sample Chart Title";

            // Lejant metnine eriş ve değiştir
            Legend legend = chart.Legend;
            legend.Text = "Custom Legend Text";

            // Çalışma kitabını kaydedin
            workbook.Save("ChartTextDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


