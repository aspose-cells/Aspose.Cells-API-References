---
title: "TickLabels.Number"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TickLabels-Eigenschaft. Stellt die Formatnummer für das TickLabels-Objekt dar"
type: docs
url: /de/net/aspose.cells.charts/ticklabels/number/
---
## TickLabels.Number property

Stellt die Formatnummer für das TickLabels‑Objekt dar.

```csharp
public int Number { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Tick-Labels konfigurieren
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.Number = 2; // Demonstrate Number property
            tickLabels.NumberFormat = "0.00";

            // Speichere die Arbeitsmappe
            workbook.Save("TickLabelsNumberDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


