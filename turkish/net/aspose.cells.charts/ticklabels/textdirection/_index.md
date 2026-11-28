---
title: "TickLabels.TextDirection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TickLabels özelliği. Metin okuma sırasını temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/ticklabels/textdirection/
---
## TickLabels.TextDirection property

Metin okuma sırasını temsil eder.

```csharp
[Obsolete("Use TickLabels.ReadingOrder property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextDirectionType TextDirection { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen TickLabels.ReadingOrder özelliğini kullanın. Bu özellik, Mart 2020'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyTextDirectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Tick etiketlerinin metin yönünü yapılandır
            Axis valueAxis = chart.ValueAxis;
            TickLabels tickLabels = valueAxis.TickLabels;
            tickLabels.TextDirection = TextDirectionType.LeftToRight;

            workbook.Save("TickLabelsTextDirectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


