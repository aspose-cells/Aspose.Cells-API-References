---
title: "ChartPoint.GetBottomPointCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ChartPoint. Ottiene il numero di punti inferiori dopo le chiamate al metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/getbottompointcount/
---
## ChartPoint.GetBottomPointCount method

Ottiene il numero di punti inferiori dopo le chiamate al metodo Chart.Calculate().

```csharp
public int GetBottomPointCount()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetBottomPointCountDemo
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
            
            // Calcola il grafico per garantire che tutti i punti siano calcolati
            chart.Calculate();
            
            try
            {
                // Ottieni il primo punto nella prima serie
                ChartPoint point = chart.NSeries[0].Points[0];
                
                // Chiama il metodo GetBottomPointCount
                int bottomPointCount = point.GetBottomPointCount();
                
                // Visualizza il risultato
                Console.WriteLine($"Number of bottom points: {bottomPointCount}");
                
                // Mostra le coordinate dei punti inferiori
                for (int i = 0; i < bottomPointCount; i++)
                {
                    float x = point.GetBottomPointXPx(i);
                    float y = point.GetBottomPointYPx(i);
                    Console.WriteLine($"Bottom point {i}: X={x}, Y={y}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBottomPointCount method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("MethodGetBottomPointCountDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


