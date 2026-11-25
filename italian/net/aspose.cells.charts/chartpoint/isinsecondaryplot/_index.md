---
title: "ChartPoint.IsInSecondaryPlot"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ChartPoint property. Restituisce o imposta un valore che indica se questo punto dati è nella seconda torta o barra in un grafico torta‑torta o barra‑torta"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/isinsecondaryplot/
---
## ChartPoint.IsInSecondaryPlot property

Ottiene o imposta un valore che indica se questo punto dati è nella seconda pie o barra su una pie di pie o barra di pie chart.

```csharp
public bool IsInSecondaryPlot { get; set; }
```

### Esempi

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

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Crea un grafico a torta che supporta trame secondarie
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configura la trama secondaria
            chart.NSeries[0].Points[2].IsInSecondaryPlot = true;
            chart.NSeries[0].Points[3].IsInSecondaryPlot = true;

            // Salva l'output
            workbook.Save("PieChartWithSecondaryPlot.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


