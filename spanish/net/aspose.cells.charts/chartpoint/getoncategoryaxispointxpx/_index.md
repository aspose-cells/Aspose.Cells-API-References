---
title: "ChartPoint.GetOnCategoryAxisPointXPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ChartPoint. Obtiene la coordenada x del punto en el eje de categorías después de llamar al método Chart.Calculate. Solo se aplica al gráfico de área"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/getoncategoryaxispointxpx/
---
## ChartPoint.GetOnCategoryAxisPointXPx method

Obtiene la coordenada x del punto en el eje de categorías después de llamar al método Chart.Calculate(). Solo se aplica al gráfico de área.

```csharp
public float GetOnCategoryAxisPointXPx(int index)
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

    public class ChartPointMethodGetOnCategoryAxisPointXPxWithInt32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular gráfico
            chart.Calculate();

            try
            {
                // Obtener el primer punto del gráfico
                ChartPoint point = chart.NSeries[0].Points[0];

                // Llamar a GetOnCategoryAxisPointXPx con el índice 0
                float xPosition = point.GetOnCategoryAxisPointXPx(0);

                // Mostrar el resultado
                Console.WriteLine($"X position of first category axis point: {xPosition} pixels");

                // Guarda el libro de trabajo
                workbook.Save("ChartPointGetOnCategoryAxisPointXPxDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOnCategoryAxisPointXPx method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


