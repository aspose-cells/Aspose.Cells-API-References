---
title: "ChartPoint.GetTopPointCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ChartPoint. Obtiene el número de puntos superiores después de llamar al método Chart.Calculate"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/gettoppointcount/
---
## ChartPoint.GetTopPointCount method

Obtiene el número de puntos superiores después de llamar al método Chart.Calculate().

```csharp
public int GetTopPointCount()
```

### Ejemplos

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

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcule el gráfico para asegurar que todas las propiedades estén configuradas
            chart.Calculate();

            try
            {
                // Obtenga el primer punto de la primera serie
                ChartPoint point = chart.NSeries[0].Points[0];
                
                // Llamar al método GetTopPointCount
                int topPointCount = point.GetTopPointCount();
                
                // Mostrar el resultado
                Console.WriteLine($"Number of top points: {topPointCount}");
                
                // Demostrar la obtención de las coordenadas del punto superior
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
            
            // Guardar el resultado
            workbook.Save("MethodGetTopPointCountDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


