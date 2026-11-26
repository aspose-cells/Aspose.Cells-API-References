---
title: "ChartPoint.InnerArcEndPointYPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene la coordenada y del punto final de la sección del pastel después de llamar al método Chart.Calculate. Se aplica al gráfico Doughnut."
type: docs
url: /es/net/aspose.cells.charts/chartpoint/innerarcendpointypx/
---
## ChartPoint.InnerArcEndPointYPx property

Obtiene la coordenada y del punto final de la sección de pastel después de llamar al método Chart.Calculate(). Se aplica al gráfico de dona.

```csharp
public float InnerArcEndPointYPx { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcEndPointYPxDemo
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
            worksheet.Cells["B2"].PutValue(40);
            worksheet.Cells["B3"].PutValue(35);
            worksheet.Cells["B4"].PutValue(25);

            // Agregar un gráfico de anillo
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcula el gráfico para obtener las propiedades del punto del gráfico
            chart.Calculate();

            // Obtén el primer punto del gráfico de la primera serie
            ChartPoint point = chart.NSeries[0].Points[0];

            // Muestra el valor actual de InnerArcEndPointYPx
            Console.WriteLine("Current InnerArcEndPointYPx value: " + point.InnerArcEndPointYPx);

            // Nota: InnerArcEndPointYPx es de solo lectura, por lo que no podemos establecerlo directamente
            // Para cambiar la posición, necesitamos modificar el tamaño del agujero del donut
            chart.NSeries[0].DoughnutHoleSize = 60; // Change hole size to affect inner arc position

            // Recalcula el gráfico para actualizar las propiedades
            chart.Calculate();

            // Muestra el nuevo valor de InnerArcEndPointYPx después de cambiar el tamaño del agujero
            Console.WriteLine("New InnerArcEndPointYPx value after changing hole size: " + point.InnerArcEndPointYPx);

            // Guarda el libro de trabajo
            workbook.Save("ChartPointPropertyInnerArcEndPointYPxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


