---
title: "TickLabels.Number"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TickLabels-egenskap. Representerar formatnumret för TickLabels-objektet"
type: docs
url: /sv/net/aspose.cells.charts/ticklabels/number/
---
## TickLabels.Number property

Representerar formatnumret för TickLabels‑objektet.

```csharp
public int Number { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Konfigurera tick-etiketter
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.Number = 2; // Demonstrate Number property
            tickLabels.NumberFormat = "0.00";

            // Spara arbetsboken
            workbook.Save("TickLabelsNumberDemo.xlsx");
        }
    }
}
```

### Se även

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


