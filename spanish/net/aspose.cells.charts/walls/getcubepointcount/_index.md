---
title: "Walls.GetCubePointCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Walls. Obtiene el número de puntos del cubo después de llamar al método Chart.Calculate"
type: docs
url: /es/net/aspose.cells.charts/walls/getcubepointcount/
---
## Walls.GetCubePointCount method

Obtiene el número de puntos del cubo después de llamar al método Chart.Calculate().

```csharp
public int GetCubePointCount()
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular el gráfico para asegurar que las propiedades de Wall estén disponibles
            chart.Calculate();

            try
            {
                // Obtener el objeto Walls
                Walls walls = chart.Walls;
                
                // Llamar al método GetCubePointCount
                int pointCount = walls.GetCubePointCount();
                
                // Mostrar el resultado
                Console.WriteLine($"Number of cube points in chart walls: {pointCount}");
                
                // Guarda el libro de trabajo
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

### Ver también

* class [Walls](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


