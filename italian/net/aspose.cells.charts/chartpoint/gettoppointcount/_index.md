---
title: "ChartPoint.GetTopPointCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ChartPoint. Ottiene il numero di punti superiori dopo aver chiamato il metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/gettoppointcount/
---
## ChartPoint.GetTopPointCount method

Ottiene il numero di punti superiori dopo aver chiamato il metodo Chart.Calculate().

```csharp
public int GetTopPointCount()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetTopPointCountDemo
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

            // Aggiungi un grafico a colonne
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per assicurarsi che tutte le proprietà siano impostate
            chart.Calculate();

            try
            {
                // Ottieni il primo punto nella prima serie
                ChartPoint point = chart.NSeries[0].Points[0];
                
                // Chiama il metodo GetTopPointCount
                int topPointCount = point.GetTopPointCount();
                
                // Visualizza il risultato
                Console.WriteLine($"Number of top points: {topPointCount}");
                
                // Dimostra come ottenere le coordinate del punto superiore
                if (topPointCount > 0)
                {
                    for (int i = 0; i < topPointCount; i++)
                    {
                        float x = point.GetTopPointXPx(i);
                        float y = point.GetTopPointYPx(i);
                        Console.WriteLine($"Top point {i + 1} coordinates: ({x}, {y})");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTopPointCount method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("MethodGetTopPointCountDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


