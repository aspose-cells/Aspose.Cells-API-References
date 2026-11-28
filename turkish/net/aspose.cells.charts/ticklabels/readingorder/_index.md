---
title: "TickLabels.ReadingOrder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TickLabels özelliği. Metin okuma sırasını temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/ticklabels/readingorder/
---
## TickLabels.ReadingOrder property

Metin okuma sırasını temsil eder.

```csharp
public TextDirectionType ReadingOrder { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyReadingOrderDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Tik etiketlerinin okuma sırasını ayarla
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.ReadingOrder = TextDirectionType.RightToLeft;

            // Çalışma kitabını kaydedin
            workbook.Save("TickLabelsReadingOrderDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


