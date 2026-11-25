---
title: "Walls.GetCubePointCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Walls. Ottiene il numero di punti del cubo dopo le chiamate al metodo Chart.Calculate"
type: docs
url: /it/net/aspose.cells.charts/walls/getcubepointcount/
---
## Walls.GetCubePointCount method

Ottiene il numero di punti del cubo dopo le chiamate al metodo Chart.Calculate().

```csharp
public int GetCubePointCount()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class WallsMethodGetCubePointCountDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per garantire che le proprietà Wall siano disponibili
            chart.Calculate();

            try
            {
                // Ottieni l'oggetto Walls
                Walls walls = chart.Walls;
                
                // Chiama il metodo GetCubePointCount
                int pointCount = walls.GetCubePointCount();
                
                // Visualizza il risultato
                Console.WriteLine($"Number of cube points in chart walls: {pointCount}");
                
                // Salva la cartella di lavoro
                workbook.Save("WallsMethodGetCubePointCountDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCubePointCount method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


