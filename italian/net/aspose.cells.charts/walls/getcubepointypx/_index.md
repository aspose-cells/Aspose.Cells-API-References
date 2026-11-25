---
title: "Walls.GetCubePointYPx"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Walls. Ottiene la coordinata y del punto apex del cubo dei muri dopo le chiamate al metodo Chart.Calculate. Il numero di punti apex del cubo dei muri è otto"
type: docs
url: /it/net/aspose.cells.charts/walls/getcubepointypx/
---
## Walls.GetCubePointYPx method

Ottiene la coordinata y del punto apice del cubo delle pareti dopo le chiamate al metodo Chart.Calculate(). Il numero di punti apice del cubo delle pareti è otto.

```csharp
public float GetCubePointYPx(int index)
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class WallsMethodGetCubePointYPxDemo
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

            // Aggiungi un grafico 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per garantire che le proprietà Wall siano popolate
            chart.Calculate();

            // Ottieni l'oggetto Walls
            Walls walls = chart.Walls;

            try
            {
                // Ottieni il numero di punti del cubo
                int pointCount = walls.GetCubePointCount();

                if (pointCount > 0)
                {
                    // Chiama GetCubePointYPx con il primo indice (0)
                    float yPx = walls.GetCubePointYPx(0);
                    Console.WriteLine($"Y-coordinate of first cube point in pixels: {yPx}");
                }
                else
                {
                    Console.WriteLine("No cube points available in the walls.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCubePointYPx method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("WallsMethodGetCubePointYPxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


