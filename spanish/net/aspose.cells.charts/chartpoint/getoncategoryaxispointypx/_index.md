---
title: "ChartPoint.GetOnCategoryAxisPointYPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ChartPoint. Obtiene la coordenada y del punto en el eje de categorías después de llamar al método Chart.Calculate. Solo se aplica al gráfico de área"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/getoncategoryaxispointypx/
---
## ChartPoint.GetOnCategoryAxisPointYPx method

Obtiene la coordenada y del punto en el eje de categorías después de llamar al método Chart.Calculate(). Solo se aplica a gráficos de Área.

```csharp
public float GetOnCategoryAxisPointYPx(int index)
```

### Observaciones

Gráfico de área 2D: el índice es 0. Gráfico de área 3D: el índice es 0 o 1.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointMethodGetOnCategoryAxisPointYPxWithInt32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 10);
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
                // Llamar a GetOnCategoryAxisPointYPx con el índice 0
                float yPx = point.GetOnCategoryAxisPointYPx(0);
                
                // Mostrar el resultado
                Console.WriteLine($"Y coordinate of point on category axis: {yPx} pixels");
                
                // Guarda el libro de trabajo
                workbook.Save("ChartPointGetOnCategoryAxisPointYPxDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointYPx method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


