---
title: "ChartPoint.GetBottomPointXPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ChartPoint. Obtiene la coordenada x del punto inferior de la forma después de llamar al método Chart.Calculate. Se aplica a gráficos 3D Column3D Bar3D Cone Cylinder Pyramid"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/getbottompointxpx/
---
## ChartPoint.GetBottomPointXPx method

Obtiene la coordenada x del punto inferior de la forma después de llamar al método Chart.Calculate(). Se aplica a los gráficos 3D: Column3D, Bar3D, Cone, Cylinder, Pyramid.

```csharp
public float GetBottomPointXPx(int index)
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetBottomPointXPxWithInt32Demo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular el gráfico para asegurar que todas las propiedades de posición estén establecidas
            chart.Calculate();

            try
            {
                // Obtener el primer punto del gráfico de la primera serie
                ChartPoint point = chart.NSeries[0].Points[0];

                // Obtener el número de puntos inferiores
                int bottomPointCount = point.GetBottomPointCount();

                if (bottomPointCount > 0)
                {
                    // Llamar a GetBottomPointXPx con el índice 0
                    float xPos = point.GetBottomPointXPx(0);
                    Console.WriteLine($"X position of bottom point (pixels): {xPos}");
                }
                else
                {
                    Console.WriteLine("No bottom points available for this chart point");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBottomPointXPx method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("ChartPointMethodGetBottomPointXPxWithInt32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


