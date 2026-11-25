---
title: "Series.LeaderLines"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Rappresenta le linee guida su un grafico. Le linee guida collegano le etichette dei dati ai punti dati. Questo oggetto non è una collezione, non esiste alcun oggetto che rappresenti una singola linea guida"
type: docs
url: /it/net/aspose.cells.charts/series/leaderlines/
---
## Series.LeaderLines property

Rappresenta le linee guida in un grafico. Le linee guida collegano le etichette dei dati ai punti dati. Questo oggetto non è una collezione; non esiste un oggetto che rappresenti una singola linea guida.

```csharp
public Line LeaderLines { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyLeaderLinesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico a torta
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configura le etichette dei dati
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShowPercentage = true;
            series.DataLabels.Position = LabelPositionType.OutsideEnd;

            // Configura le linee guida
            series.HasLeaderLines = true;
            series.LeaderLines.IsAuto = false;
            series.LeaderLines.Style = LineType.Dot;
            series.LeaderLines.WeightPt = 1.5;
            series.LeaderLines.Color = Color.Blue;

            // Salva la cartella di lavoro
            workbook.Save("SeriesPropertyLeaderLinesDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


