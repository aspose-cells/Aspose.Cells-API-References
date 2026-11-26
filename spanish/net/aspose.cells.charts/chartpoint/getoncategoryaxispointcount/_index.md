---
title: "ChartPoint.GetOnCategoryAxisPointCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ChartPoint. Obtiene el número de puntos en el eje de categorías después de llamar al método Chart.Calculate. Solo se aplica a gráficos de área"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/getoncategoryaxispointcount/
---
## ChartPoint.GetOnCategoryAxisPointCount method

Obtiene el número de puntos en el eje de categorías después de llamar al método Chart.Calculate(). Solo se aplica a los gráficos de área.

```csharp
public int GetOnCategoryAxisPointCount()
```

### Observaciones

El gráfico de área 2D devuelve 1, el gráfico de área 3D devuelve 2.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetOnCategoryAxisPointCountDemo
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

            // Agregar un gráfico de área
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular el gráfico para asegurar que todos los puntos del gráfico estén calculados
            chart.Calculate();

            try
            {
                // Obtener el primer punto del gráfico de la primera serie
                ChartPoint point = chart.NSeries[0].Points[0];
                
                // Llamar al método GetOnCategoryAxisPointCount
                int pointCount = point.GetOnCategoryAxisPointCount();
                
                Console.WriteLine($"Number of points on category axis: {pointCount}");
                
                // Mostrar las coordenadas de cada punto en el eje de categorías
                for (int i = 0; i < pointCount; i++)
                {
                    float x = point.GetOnCategoryAxisPointXPx(i);
                    float y = point.GetOnCategoryAxisPointYPx(i);
                    Console.WriteLine($"Point {i}: X={x}, Y={y}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointCount method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("MethodGetOnCategoryAxisPointCountDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


