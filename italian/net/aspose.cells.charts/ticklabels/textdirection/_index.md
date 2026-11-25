---
title: "TickLabels.TextDirection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TickLabels. Rappresenta l'ordine di lettura del testo"
type: docs
url: /it/net/aspose.cells.charts/ticklabels/textdirection/
---
## TickLabels.TextDirection property

Rappresenta l'ordine di lettura del testo.

```csharp
[Obsolete("Use TickLabels.ReadingOrder property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextDirectionType TextDirection { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà TickLabels.ReadingOrder. Questa proprietà sarà rimossa 12 mesi dopo a partire da marzo 2020. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

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

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configura la direzione del testo delle etichette dei tick
            Axis valueAxis = chart.ValueAxis;
            TickLabels tickLabels = valueAxis.TickLabels;
            tickLabels.TextDirection = TextDirectionType.LeftToRight;

            workbook.Save("TickLabelsTextDirectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


