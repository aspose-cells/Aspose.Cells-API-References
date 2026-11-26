---
title: "Walls.GetCubePointXPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Walls. Obtiene la coordenada x del punto ápex del cubo de walls después de llamar al método Chart.Calculate. El número de puntos ápex del cubo de walls es ocho."
type: docs
url: /es/net/aspose.cells.charts/walls/getcubepointxpx/
---
## Walls.GetCubePointXPx method

Obtiene la coordenada x del punto ápex del cubo de paredes después de llamar al método Chart.Calculate(). El número de puntos ápex del cubo de paredes es ocho.

```csharp
public float GetCubePointXPx(int index)
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
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

            // Cree un gráfico 3D.
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Calcular el gráfico para asegurar que las propiedades de Wall estén disponibles
            chart.Calculate();

            // Obtener el objeto Walls
            Walls walls = chart.Walls;

            try
            {
                // Obtenga el recuento de puntos del cubo.
                int pointCount = walls.GetCubePointCount();

                if (pointCount > 0)
                {
                    // Llame a GetCubePointXPx con el índice 0 (primer punto).
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

            // Guarda el libro de trabajo
            workbook.Save("WallsMethodGetCubePointXPxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


