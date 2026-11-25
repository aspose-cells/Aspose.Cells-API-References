---
title: "ChartPointCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ChartPointCollection. Rimuove il punto all'indice della serie"
type: docs
url: /it/net/aspose.cells.charts/chartpointcollection/removeat/
---
## ChartPointCollection.RemoveAt method

Rimuove il punto all'indice della serie.

```csharp
public void RemoveAt(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice del punto. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointCollectionMethodRemoveAtWithInt32Demo
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

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni la collezione dei punti della prima serie
            ChartPointCollection points = chart.NSeries[0].Points;

            try
            {
                // Visualizza il conteggio iniziale
                Console.WriteLine($"Initial points count: {points.Count}");

                // Rimuovi il punto all'indice 1 (secondo punto)
                points.RemoveAt(1);

                // Visualizza il risultato
                Console.WriteLine($"Points count after RemoveAt: {points.Count}");
                Console.WriteLine("Point at index 1 removed successfully.");

                // Salva la cartella di lavoro
                workbook.Save("ChartPointCollectionRemoveAtDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


