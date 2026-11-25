---
title: "Enum CrossType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.CrossType enum. Rappresenta il tipo di incrocio dell'asse"
type: docs
url: /it/net/aspose.cells.charts/crosstype/
---
## CrossType enumeration

Rappresenta il tipo di intersezione dell'asse.

```csharp
public enum CrossType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Automatic | `0` | Microsoft Excel imposta il punto di incrocio dell'asse. |
| Maximum | `1` | L'asse incrocia al valore massimo. |
| Minimum | `2` | L'asse interseca al valore minimo. |
| Custom | `3` | L'asse interseca al valore personalizzato. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CrossTypeDemo
    {
        public static void CrossTypeExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            // Aggiunta di un nuovo foglio di lavoro all'oggetto Excel
            int sheetIndex = workbook.Worksheets.Add();
            // Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Aggiunta di valori di esempio alle celle
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Aggiunta di un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            // Accesso all'istanza del grafico appena aggiunto
            Chart chart = worksheet.Charts[chartIndex];
            // Aggiunta di NSeries (origine dati del grafico) al grafico dall'intervallo di celle "A1" a "B3"
            chart.NSeries.Add("A1:B3", true);

            // Imposta il valore massimo dell'asse dei valori
            chart.ValueAxis.MaxValue = 200;
            // Imposta il valore minimo dell'asse dei valori
            chart.ValueAxis.MinValue = 0;
            // Imposta l'unità principale
            chart.ValueAxis.MajorUnit = 25;

            // L'asse Category(X) interseca al valore massimo
            chart.ValueAxis.CrossType = CrossType.Maximum;

            // Imposta il numero di categorie o serie tra le etichette dei segni di graduazione
            chart.CategoryAxis.TickLabelSpacing = 2;

            // Salvataggio del file Excel
            workbook.Save("CrossTypeExample.xlsx");
            workbook.Save("CrossTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


