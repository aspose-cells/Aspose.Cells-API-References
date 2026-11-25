---
title: "Classe AxisBins"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Charts.AxisBins. Rappresenta i cestini dell'asse"
type: docs
url: /it/net/aspose.cells.charts/axisbins/
---
## AxisBins class

Rappresenta i contenitori dell'asse

```csharp
public class AxisBins
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.cells.charts/axisbins/count/) { get; set; } | Ottiene o imposta il conteggio dei cestini dell'asse |
| [IsAutomatic](../../aspose.cells.charts/axisbins/isautomatic/) { get; set; } | Indica se i cestini dell'asse sono automatici. |
| [IsByCategory](../../aspose.cells.charts/axisbins/isbycategory/) { get; set; } | Indica se il raggruppamento dei dati per categoria è abilitato. |
| [Overflow](../../aspose.cells.charts/axisbins/overflow/) { get; set; } | Ottiene o imposta l'overflow dei cestini dell'asse |
| [Underflow](../../aspose.cells.charts/axisbins/underflow/) { get; set; } | Ottiene o imposta l'underflow dei cestini dell'asse |
| [Width](../../aspose.cells.charts/axisbins/width/) { get; set; } | Ottiene o imposta la larghezza del cestino dell'asse. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ResetOverflow](../../aspose.cells.charts/axisbins/resetoverflow/)() | (**Obsolete.**) Reimposta l'overflow |
| [ResetUnderflow](../../aspose.cells.charts/axisbins/resetunderflow/)() | (**Obsolete.**) Reimposta l'underflow |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisBinsDemo
    {
        public static void AxisBinsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            // Aggiungi un nuovo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Histogram, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi serie di dati al grafico
            chart.NSeries.Add("A1:A5", true);

            // Accedi all'asse dei valori
            Axis valueAxis = chart.ValueAxis;

            // Accedi ai cestini dell'asse dei valori
            AxisBins bins = valueAxis.Bins;

            // Imposta le proprietà per i cestini
            bins.IsByCategory = false;
            bins.IsAutomatic = true;
            bins.Width = 10.0;
            bins.Count = 5;
            bins.Overflow = 60.0;
            bins.Underflow = 0.0;

            // Reimposta l'overflow e l'underflow
            //bins.ResetOverflow();
            //bins.ResetUnderflow();

            // Salva la cartella di lavoro
            workbook.Save("AxisBinsExample.xlsx");
            workbook.Save("AxisBinsExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


