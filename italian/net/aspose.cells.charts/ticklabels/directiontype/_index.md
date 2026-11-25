---
title: "TickLabels.DirectionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TickLabels. Ottiene e imposta la direzione del testo"
type: docs
url: /it/net/aspose.cells.charts/ticklabels/directiontype/
---
## TickLabels.DirectionType property

Ottiene e imposta la direzione del testo.

```csharp
public ChartTextDirectionType DirectionType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyDirectionTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].Value = 50;
            worksheet.Cells["A2"].Value = 100;
            worksheet.Cells["A3"].Value = 150;
            worksheet.Cells["A4"].Value = 200;
            worksheet.Cells["B1"].Value = 60;
            worksheet.Cells["B2"].Value = 32;
            worksheet.Cells["B3"].Value = 50;
            worksheet.Cells["B4"].Value = 40;
            worksheet.Cells["C1"].Value = "清华";
            worksheet.Cells["C2"].Value = "北大";
            worksheet.Cells["C3"].Value = "人大";
            worksheet.Cells["C4"].Value = "科大";

            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta i dati del grafico
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Imposta la direzione delle etichette dei tick a verticale
            chart.CategoryAxis.TickLabels.DirectionType = ChartTextDirectionType.Vertical;

            // Salva la cartella di lavoro
            workbook.Save("TickLabelsDirectionTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ChartTextDirectionType](../../charttextdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


