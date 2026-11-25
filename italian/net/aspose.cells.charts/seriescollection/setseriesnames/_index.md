---
title: "SeriesCollection.SetSeriesNames"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SeriesCollection. Imposta i nomi di tutte le serie nel grafico"
type: docs
url: /it/net/aspose.cells.charts/seriescollection/setseriesnames/
---
## SeriesCollection.SetSeriesNames method

Imposta i nomi di tutte le serie nel grafico.

```csharp
public void SetSeriesNames(int startIndex, string area, bool isVertical)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | Int32 | L'indice della prima serie di cui vuoi impostare il nome. |
| area | String | Specifica l'area per il nome della serie. |
| isVertical | Booleano | &gt;Specifica se tracciare la serie da un intervallo di valori di cella per riga o per colonna. |

### Osservazioni

Se l'indice iniziale è maggiore del numero delle serie, l'operazione terminerà senza fare nulla. Se imposti i dati su celle contigue, usa i due punti per separarle. Ad esempio, $C$2:$C$5. Se imposti i dati su celle contigue, usa la virgola per separarle. Ad esempio, ($C$2,$D$5).

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionMethodSetSeriesNamesWithInt32StringBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Q1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["C1"].PutValue("Q2");
            worksheet.Cells["C2"].PutValue(120);
            worksheet.Cells["C3"].PutValue(180);
            worksheet.Cells["C4"].PutValue(220);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ottieni la collezione di serie del grafico
            SeriesCollection seriesCollection = chart.NSeries;

            try
            {
                // Chiama SetSeriesNames con i parametri (startIndex: 0, area: "A2:A4", isVertical: true)
                seriesCollection.SetSeriesNames(0, "A2:A4", true);

                // Aggiungi dati della serie
                seriesCollection.Add("B2:C4", true);

                Console.WriteLine("SetSeriesNames method executed successfully with parameters (Int32, String, Boolean)");
                Console.WriteLine("Series names set from range A2:A4");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetSeriesNames method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("SeriesCollectionMethodSetSeriesNamesWithInt32StringBooleanDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


