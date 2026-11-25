---
title: "SeriesCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SeriesCollection. Rimuove una serie all'indice specifico"
type: docs
url: /it/net/aspose.cells.charts/seriescollection/removeat/
---
## SeriesCollection.RemoveAt method

Rimuove una serie all'indice specifico.

```csharp
public void RemoveAt(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B1:B4", true);
            chart.NSeries.Add("C1:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Chiama RemoveAt per rimuovere la prima serie (indice 0)
                chart.NSeries.RemoveAt(0);
                
                Console.WriteLine("Series at index 0 removed successfully");
                
                // Verifica il conteggio delle serie rimanenti
                Console.WriteLine($"Remaining series count: {chart.NSeries.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("SeriesCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


