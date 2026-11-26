---
title: "ChartPoint.GetBottomPointCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ChartPoint. Obtiene el número de puntos inferiores después de llamar al método Chart.Calculate"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/getbottompointcount/
---
## ChartPoint.GetBottomPointCount method

Obtiene el número de puntos inferiores después de llamar al método Chart.Calculate().

```csharp
public int GetBottomPointCount()
```

### Ejemplos

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
            
            // Calcular el gráfico para asegurar que todos los puntos estén calculados
            chart.Calculate();
            
            try
            {
                // Obtenga el primer punto de la primera serie
                ChartPoint point = chart.NSeries[0].Points[0];
                
                // Llame al método GetBottomPointCount
                int bottomPointCount = point.GetBottomPointCount();
                
                // Mostrar el resultado
                Console.WriteLine($"Number of bottom points: {bottomPointCount}");
                
                // Muestre las coordenadas de los puntos inferiores
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
            
            // Guardar el resultado
            workbook.Save("MethodGetBottomPointCountDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


