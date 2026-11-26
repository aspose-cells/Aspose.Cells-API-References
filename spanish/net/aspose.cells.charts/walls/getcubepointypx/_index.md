---
title: "Walls.GetCubePointYPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Walls. Obtiene la coordenada y del punto ápex del cubo de paredes después de llamar al método Chart.Calculate. El número de puntos ápex del cubo de paredes es ocho"
type: docs
url: /es/net/aspose.cells.charts/walls/getcubepointypx/
---
## Walls.GetCubePointYPx method

Obtiene la coordenada y del punto ápex del cubo de paredes después de llamar al método Chart.Calculate(). El número de puntos ápex del cubo de paredes es ocho.

```csharp
public float GetCubePointYPx(int index)
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular el gráfico para asegurar que las propiedades de Wall se completen
            chart.Calculate();

            // Obtener el objeto Walls
            Walls walls = chart.Walls;

            try
            {
                // Obtener el número de puntos del cubo
                int pointCount = walls.GetCubePointCount();

                if (pointCount > 0)
                {
                    // Llamar a GetCubePointYPx con el primer índice (0)
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

            // Guarda el libro de trabajo
            workbook.Save("WallsMethodGetCubePointYPxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


