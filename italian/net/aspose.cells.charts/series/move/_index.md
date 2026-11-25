---
title: "Series.Move"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Series. Sposta la serie verso l'alto o verso il basso"
type: docs
url: /it/net/aspose.cells.charts/series/move/
---
## Series.Move method

Sposta la serie su o giù.

```csharp
public void Move(int count)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| conteggio | Int32 | Il numero di spostamenti verso l'alto o verso il basso. Sposta la serie verso l'alto se questo valore è inferiore a zero; sposta la serie verso il basso se è superiore a zero. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesMethodMoveWithInt32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie al grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Ottieni la prima serie
            Series series = chart.NSeries[0];
            
            try
            {
                // Chiama il metodo Move con parametro Int32
                series.Move(1);
                
                Console.WriteLine("Series moved successfully by 1 position");
                
                // Mostra l'effetto cambiando il nome della serie
                series.Name = "Moved Series";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("SeriesMethodMoveWithInt32Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


