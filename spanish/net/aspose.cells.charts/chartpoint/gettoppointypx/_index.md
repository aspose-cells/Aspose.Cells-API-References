---
title: "ChartPoint.GetTopPointYPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ChartPoint. Obtiene la coordenada y del punto superior de la forma después de llamar al método Chart.Calculate. Se aplica a gráficos 3D Column3D Bar3D Cone Cylinder Pyramid y Area3D"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/gettoppointypx/
---
## ChartPoint.GetTopPointYPx method

Obtiene la coordenada y del punto superior de la forma después de llamar al método Chart.Calculate(). Se aplica a gráficos 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid y Area3D.

```csharp
public float GetTopPointYPx(int index)
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetTopPointYPxWithInt32Demo
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
            
            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Calcular el gráfico para asegurar que todas las propiedades de posición se calculen
            chart.Calculate();
            
            // Obtener el primer punto del gráfico de la primera serie
            ChartPoint point = chart.NSeries[0].Points[0];
            
            try
            {
                // Obtenga el número de puntos superiores
                int topPointCount = point.GetTopPointCount();
                
                if (topPointCount > 0)
                {
                    // Llame a GetTopPointYPx con el índice 0
                    float yPx = point.GetTopPointYPx(0);
                    
                    Console.WriteLine($"Top point Y position in pixels: {yPx}");
                    Console.WriteLine("Method executed successfully with parameter (Int32)");
                }
                else
                {
                    Console.WriteLine("No top points available for this chart point");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTopPointYPx method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("ChartPointMethodGetTopPointYPxWithInt32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


