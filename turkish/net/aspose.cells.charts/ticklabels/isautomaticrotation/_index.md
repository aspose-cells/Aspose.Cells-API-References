---
title: "TickLabels.IsAutomaticRotation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TickLabels özelliği. Döndürme açısının otomatik olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.charts/ticklabels/isautomaticrotation/
---
## TickLabels.IsAutomaticRotation property

Dönüş açısının otomatik olup olmadığını gösterir

```csharp
public bool IsAutomaticRotation { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyIsAutomaticRotationDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Tick etiketlerini yapılandır
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.IsAutomaticRotation = false; // Disable automatic rotation
            tickLabels.RotationAngle = 45; // Set manual rotation angle

            workbook.Save("TickLabelsRotationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


