---
title: "Walls.GetCubePointXPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Walls. Restituisce la coordinata x del punto apice del cubo delle pareti dopo aver chiamato il metodo Chart.Calculate. Il numero di punti apice del cubo delle pareti è otto"
type: docs
url: /it/net/aspose.cells.charts/walls/getcubepointxpx/
---
## Walls.GetCubePointXPx method

Ottiene la coordinata x del punto apice del cubo delle pareti dopo aver chiamato il metodo Chart.Calculate(). Il numero di punti apice del cubo delle pareti è otto.

```csharp
public float GetCubePointXPx(int index)
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class WallsMethodGetCubePointXPxWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            worksheet.Cells["B5"].PutValue(4000);

            // Crea un grafico 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Calcola il grafico per garantire che le proprietà Wall siano disponibili
            chart.Calculate();

            // Ottieni l'oggetto Walls
            Walls walls = chart.Walls;

            try
            {
                // Ottieni il conteggio dei punti del cubo
                int pointCount = walls.GetCubePointCount();

                if (pointCount > 0)
                {
                    // Chiama GetCubePointXPx con indice 0 (primo punto)
                    float xCoordinate = walls.GetCubePointXPx(0);
                    
                    Console.WriteLine($"X coordinate of first cube point in pixels: {xCoordinate}");
                    Console.WriteLine("Method executed successfully with parameter (Int32)");
                }
                else
                {
                    Console.WriteLine("No cube points available in the walls");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCubePointXPx method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("WallsMethodGetCubePointXPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


