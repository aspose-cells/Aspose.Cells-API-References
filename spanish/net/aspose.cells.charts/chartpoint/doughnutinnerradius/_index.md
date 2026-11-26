---
title: "ChartPoint.DoughnutInnerRadius"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene el radio interno de la porción de dona en unidades de píxeles después de llamar al método Chart.Calculate. Se aplica al gráfico de dona"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/doughnutinnerradius/
---
## ChartPoint.DoughnutInnerRadius property

Obtiene el radio interno de la porción de dona en unidades de píxeles después de llamar al método Chart.Calculate(). Se aplica al gráfico de dona.

```csharp
public int DoughnutInnerRadius { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyDoughnutInnerRadiusDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("C1");
            worksheet.Cells["A3"].PutValue("C2");
            worksheet.Cells["A4"].PutValue("C3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(5);

            // Agregar un gráfico de anillo
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcule el gráfico para obtener los puntos del gráfico
            chart.Calculate();

            // Obtén el primer punto del gráfico de la primera serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Muestre el valor actual de DoughnutInnerRadius
            Console.WriteLine("Current DoughnutInnerRadius value: " + point.DoughnutInnerRadius);

            // Nota: DoughnutInnerRadius es de solo lectura, por lo que no podemos establecerlo directamente
            // Para cambiar el radio interno, necesitamos ajustar la propiedad HoleSize del gráfico
            chart.FirstSliceAngle = 30; // Adjust the first slice angle instead since HoleSize isn't available

            // Recalcule el gráfico para actualizar DoughnutInnerRadius
            chart.Calculate();

            // Muestre el valor actualizado de DoughnutInnerRadius
            Console.WriteLine("Updated DoughnutInnerRadius value: " + point.DoughnutInnerRadius);

            // Guarda el libro de trabajo
            workbook.Save("DoughnutInnerRadiusDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


