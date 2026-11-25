---
title: "TickLabels.ReadingOrder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TickLabels. Rappresenta l'ordine di lettura del testo"
type: docs
url: /it/net/aspose.cells.charts/ticklabels/readingorder/
---
## TickLabels.ReadingOrder property

Rappresenta l'ordine di lettura del testo.

```csharp
public TextDirectionType ReadingOrder { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyReadingOrderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Imposta l'ordine di lettura delle etichette di tick
            TickLabels tickLabels = chart.ValueAxis.TickLabels;
            tickLabels.ReadingOrder = TextDirectionType.RightToLeft;

            // Salva la cartella di lavoro
            workbook.Save("TickLabelsReadingOrderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


