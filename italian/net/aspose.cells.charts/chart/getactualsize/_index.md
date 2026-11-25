---
title: "Chart.GetActualSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Chart. Ottiene le dimensioni effettive del grafico in unità di pixel"
type: docs
url: /it/net/aspose.cells.charts/chart/getactualsize/
---
## Chart.GetActualSize method

Ottiene la dimensione reale del grafico in unità di pixel.

```csharp
public int[] GetActualSize()
```

### Valore di ritorno

Dimensione effettiva in un array (larghezza e altezza). [0] è la larghezza; [1] è l'altezza.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodGetActualSizeDemo
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
            
            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:B4", true);
            
            try
            {
                // Chiama il metodo GetActualSize
                int[] actualSize = chart.GetActualSize();
                
                // Visualizza il risultato
                Console.WriteLine($"Actual chart size - Width: {actualSize[0]}px, Height: {actualSize[1]}px");
                
                // Mostra l'effetto ridimensionando l'oggetto grafico
                chart.ChartObject.Width = actualSize[0];
                chart.ChartObject.Height = actualSize[1];
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetActualSize method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("ChartMethodGetActualSizeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


