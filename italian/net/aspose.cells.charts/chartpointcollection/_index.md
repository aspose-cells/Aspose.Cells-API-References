---
title: "Classe ChartPointCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Charts.ChartPointCollection. Rappresenta una collezione che contiene tutti i punti in una serie"
type: docs
url: /it/net/aspose.cells.charts/chartpointcollection/
---
## ChartPointCollection class

Rappresenta una raccolta che contiene tutti i punti in una serie.

```csharp
public class ChartPointCollection : IEnumerable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.cells.charts/chartpointcollection/count/) { get; } | Ottiene il conteggio del punto del grafico. |
| [Item](../../aspose.cells.charts/chartpointcollection/item/) { get; } | Ottiene l'elemento [`ChartPoint`](../chartpoint/) all'indice specificato nella serie. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Clear](../../aspose.cells.charts/chartpointcollection/clear/)() | Rimuove tutte le impostazioni dei punti del grafico. |
| [GetEnumerator](../../aspose.cells.charts/chartpointcollection/getenumerator/)() | Restituisce un enumeratore per l'intera `ChartPointCollection`. |
| [RemoveAt](../../aspose.cells.charts/chartpointcollection/removeat/)(int) | Rimuove il punto all'indice della serie. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointCollectionDemo
    {
        public static void ChartPointCollectionExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();

            // Ottenere il riferimento del primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiunta di valori di esempio alle celle
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Aggiunta di un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.PieExploded, 5, 0, 25, 10);

            // Accesso all'istanza del grafico appena aggiunto
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiunta di NSeries (origine dati del grafico) al grafico dall'intervallo di celle "A1" a "B3"
            chart.NSeries.Add("A1:B3", true);

            // Mostra etichette dati 
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Accesso a ChartPointCollection
            ChartPointCollection points = chart.NSeries[0].Points;

            // Iterazione attraverso i punti nella collezione
            for (int i = 0; i < points.Count; i++)
            {
                // Ottieni punto dati
                ChartPoint point = points[i];
                
                // Imposta esplosione della torta
                point.Explosion = 15;
                
                // Imposta colore del bordo
                point.Border.Color = System.Drawing.Color.Red;
            }

            // Salvataggio del file Excel
            workbook.Save("ChartPointCollectionExample.xlsx");
            workbook.Save("ChartPointCollectionExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


