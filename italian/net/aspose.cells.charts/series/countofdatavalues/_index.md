---
title: "Series.CountOfDataValues"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Ottiene il numero dei valori dei dati"
type: docs
url: /it/net/aspose.cells.charts/series/countofdatavalues/
---
## Series.CountOfDataValues property

Ottiene il numero dei valori dei dati.

```csharp
public int CountOfDataValues { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyCountOfDataValuesDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            for (int i = 0; i < 4; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1); // A1:A4 with values 1-4
            }

            // Crea un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie utilizzando l'intervallo di dati
            chart.NSeries.Add("A1:A4", true);
            
            // Visualizza il conteggio dei valori dei dati nella prima serie
            Console.WriteLine("Count of data values in series: " + chart.NSeries[0].CountOfDataValues);
            
            // Salva la cartella di lavoro
            workbook.Save("SeriesPropertyCountOfDataValuesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


