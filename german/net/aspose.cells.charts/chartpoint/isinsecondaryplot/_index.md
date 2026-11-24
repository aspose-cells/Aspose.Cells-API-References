---
title: "ChartPoint.IsInSecondaryPlot"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartPoint-Eigenschaft. Gibt einen Wert zurück oder setzt ihn, der angibt, ob dieser Datenpunkt im zweiten Kreis oder Balken eines Kreis‑in‑Kreis‑ oder Balken‑in‑Kreis‑Diagramms liegt."
type: docs
url: /de/net/aspose.cells.charts/chartpoint/isinsecondaryplot/
---
## ChartPoint.IsInSecondaryPlot property

Ermittelt oder legt einen Wert fest, der angibt, ob dieser Datenpunkt im zweiten Kuchen‑ oder Balken eines Kuchen‑in‑Kuchen‑ oder Balken‑in‑Kuchen‑Diagramms liegt.

```csharp
public bool IsInSecondaryPlot { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyIsInSecondaryPlotDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Erstelle ein Kreisdiagramm, das sekundäre Diagramme unterstützt.
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Konfiguriere das sekundäre Diagramm.
            chart.NSeries[0].Points[2].IsInSecondaryPlot = true;
            chart.NSeries[0].Points[3].IsInSecondaryPlot = true;

            // Ausgabe speichern
            workbook.Save("PieChartWithSecondaryPlot.xlsx");
        }
    }
}
```

### Siehe auch

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


