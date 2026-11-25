---
title: "DataLabels.ShowSeriesName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataLabels. Indica se il nome della serie viene visualizzato sulle etichette dati in un grafico. True per mostrare il nome della serie. False per nasconderlo"
type: docs
url: /it/net/aspose.cells.charts/datalabels/showseriesname/
---
## DataLabels.ShowSeriesName property

Indica se il nome della serie viene visualizzato sulle etichette dati in un grafico. True per mostrare il nome della serie. False per nasconderlo.

```csharp
public bool ShowSeriesName { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowSeriesNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Aggiungi un grafico a colonne
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.Add("B1:B4", true);

            // Abilita le etichette dati per la prima serie
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;

            // Abilita la visualizzazione del nome della serie per l'etichetta dati di un punto specifico
            var points = series.Points;
            points[1].DataLabels.ShowSeriesName = true;

            // Calcola il grafico
            chart.Calculate();

            // Salva la cartella di lavoro
            workbook.Save("DataLabelsShowSeriesNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


