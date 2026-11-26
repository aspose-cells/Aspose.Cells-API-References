---
title: "ChartPoint.InnerArcEndPointXPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene la coordenada x del punto final de la sección de pastel después de llamar al método Chart.Calculate. Se aplica a gráficos Doughnut."
type: docs
url: /es/net/aspose.cells.charts/chartpoint/innerarcendpointxpx/
---
## ChartPoint.InnerArcEndPointXPx property

Obtiene la coordenada x del punto final de la sección de pastel después de llamar al método Chart.Calculate(). Se aplica a los gráficos de dona.

```csharp
public float InnerArcEndPointXPx { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcEndPointXPxDemo
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
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(2);

            // Agregar un gráfico de anillo
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcula el gráfico para obtener las propiedades del punto del gráfico
            chart.Calculate();

            // Obtén el primer punto del gráfico de la primera serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mostrar el valor actual de InnerArcEndPointXPx
            Console.WriteLine("Current InnerArcEndPointXPx value: " + point.InnerArcEndPointXPx);

            // Nota: InnerArcEndPointXPx es de solo lectura, por lo que no podemos establecerlo directamente
            // Para cambiar la posición del punto final, necesitamos modificar el tamaño del agujero del doughnut
            chart.NSeries[0].DoughnutHoleSize = 50; // Set hole size to 50%

            // Recalcula el gráfico para actualizar las propiedades
            chart.Calculate();

            // Mostrar el nuevo valor de InnerArcEndPointXPx después de cambiar el tamaño del agujero
            Console.WriteLine("New InnerArcEndPointXPx value after changing doughnut hole size: " + point.InnerArcEndPointXPx);

            // Guarda el libro de trabajo
            workbook.Save("ChartPointPropertyInnerArcEndPointXPxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


