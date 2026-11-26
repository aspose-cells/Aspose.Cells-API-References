---
title: "ChartPoint.InnerRadiusPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene el radio interno de la porción de doughnut en unidades de píxeles después de llamar al método Chart.Calculate. Se aplica al gráfico Doughnut"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/innerradiuspx/
---
## ChartPoint.InnerRadiusPx property

Obtiene el radio interno de la porción de doughnut en unidades de píxeles después de llamar al método Chart.Calculate(). Se aplica al gráfico Doughnut.

```csharp
[Obsolete("Use ChartPoint.DoughnutInnerRadius property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int InnerRadiusPx { get; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad ChartPoint.DoughnutInnerRadius. Esta propiedad será eliminada 12 meses después, a partir de junio de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerRadiusPxDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcule el gráfico para obtener las propiedades de los puntos del gráfico
            chart.Calculate();

            // Obtén el primer punto del gráfico de la primera serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Muestre el valor actual del radio interno (propiedad de solo lectura)
            Console.WriteLine("Current InnerRadiusPx value: " + point.InnerRadiusPx);

            // Nota: InnerRadiusPx es de solo lectura, por lo que no podemos establecerlo directamente
            // Para cambiar el radio interno, necesitamos ajustar el tamaño del agujero del doughnut
            chart.NSeries[0].DoughnutHoleSize = 50; // Percentage of the chart size

            // Recalcula el gráfico para actualizar las propiedades
            chart.Calculate();

            // Muestre el nuevo valor del radio interno después de cambiar el tamaño del agujero del doughnut
            Console.WriteLine("New InnerRadiusPx value after changing DoughnutHoleSize: " + point.InnerRadiusPx);

            // Guardar el resultado
            workbook.Save("ChartPointPropertyInnerRadiusPxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


