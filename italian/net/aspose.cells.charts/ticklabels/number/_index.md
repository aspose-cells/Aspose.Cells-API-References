---
title: "TickLabels.Number"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TickLabels. Rappresenta il numero di formato per l'oggetto TickLabels"
type: docs
url: /it/net/aspose.cells.charts/ticklabels/number/
---
## TickLabels.Number property

Rappresenta il numero di formato per l'oggetto TickLabels.

```csharp
public int Number { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Configura le etichette dei tick
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.Number = 2; // Demonstrate Number property
            tickLabels.NumberFormat = "0.00";

            // Salva la cartella di lavoro
            workbook.Save("TickLabelsNumberDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


