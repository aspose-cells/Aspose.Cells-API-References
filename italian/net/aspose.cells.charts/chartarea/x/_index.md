---
title: "ChartArea.X"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartArea. Ottiene o imposta lo spostamento orizzontale dalla colonna dell'angolo superiore sinistro in unità di 1/4000 dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartarea/x/
---
## ChartArea.X property

Ottiene o imposta lo spostamento orizzontale dalla colonna dell'angolo superiore sinistro, in unità di 1/4000 dell'area del grafico.

```csharp
[Obsolete("Use ChartArea.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartArea.XRatioToChart, invece. X = XRatioToChart * 4000. Questa proprietà sarà rimossa 12 mesi dopo, a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyXDemo
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

            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configura l'area del grafico
            Aspose.Cells.Charts.ChartArea chartArea = chart.ChartArea;
            chartArea.X = 10; // Demonstrating X property usage
            chartArea.Y = 10;
            chartArea.Width = 400;
            chartArea.Height = 300;

            // Salva l'output
            workbook.Save("ChartAreaXDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


