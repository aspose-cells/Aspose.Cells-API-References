---
title: "SeriesCollection.ChangeSeriesOrder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SeriesCollection. Cambia direttamente l'ordine delle due serie"
type: docs
url: /it/net/aspose.cells.charts/seriescollection/changeseriesorder/
---
## SeriesCollection.ChangeSeriesOrder method

Cambia direttamente l'ordine delle due serie.

```csharp
[Obsolete("Use SeriesCollection.SwapSeries property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ChangeSeriesOrder(int sourceIndex, int destIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceIndex | Int32 | L'indice corrente |
| destIndex | Int32 | L'indice di destinazione |

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo SeriesCollection.SwapSeries. Questo metodo sarà rimosso tra 12 mesi a partire da giugno 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionMethodChangeSeriesOrderWithInt32Int32Demo
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
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(60);
            
            worksheet.Cells["C1"].PutValue("Series 3");
            worksheet.Cells["C2"].PutValue(70);
            worksheet.Cells["C3"].PutValue(80);
            worksheet.Cells["C4"].PutValue(90);

            // Crea un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie al grafico
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            
            // Ottieni la raccolta di serie
            SeriesCollection seriesCollection = chart.NSeries;

            try
            {
                // Chiama il metodo ChangeSeriesOrder per scambiare le serie agli indici 0 e 2
                seriesCollection.ChangeSeriesOrder(0, 2);
                
                Console.WriteLine("Series order changed successfully. Series at index 0 and 2 swapped.");
                
                // Mostra il nuovo ordine delle serie
                for (int i = 0; i < seriesCollection.Count; i++)
                {
                    Console.WriteLine($"Series {i + 1}: {seriesCollection[i].Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ChangeSeriesOrder method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("ChangeSeriesOrderWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


