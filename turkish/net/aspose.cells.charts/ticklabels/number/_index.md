---
title: "TickLabels.Number"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TickLabels özelliği. TickLabels nesnesi için biçim numarasını temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/ticklabels/number/
---
## TickLabels.Number property

TickLabels nesnesi için biçim numarasını temsil eder.

```csharp
public int Number { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyNumberDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Tick etiketlerini yapılandır
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.Number = 2; // Demonstrate Number property
            tickLabels.NumberFormat = "0.00";

            // Çalışma kitabını kaydedin
            workbook.Save("TickLabelsNumberDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


