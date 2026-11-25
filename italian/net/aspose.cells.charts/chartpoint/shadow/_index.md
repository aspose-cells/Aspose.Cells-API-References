---
title: "ChartPoint.Shadow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ChartPoint property. Vero se il punto del grafico ha un'ombra"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/shadow/
---
## ChartPoint.Shadow property

Vero se il chartpoint ha un'ombra.

```csharp
public bool Shadow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyShadowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(180);

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            chart.NSeries.Add("A1:B3", true);
            
            foreach (ChartPoint point in chart.NSeries[0].Points)
            {
                point.Shadow = true;
                point.Border.Color = Color.Blue;
            }

            workbook.Save("ChartPointShadowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


