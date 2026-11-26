---
title: "ChartPoint.InnerArcStartPointYPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene la coordenada y del punto inicial de la sección del pastel después de llamar al método Chart.Calculate. Se aplica al gráfico Doughnut."
type: docs
url: /es/net/aspose.cells.charts/chartpoint/innerarcstartpointypx/
---
## ChartPoint.InnerArcStartPointYPx property

Obtiene la coordenada y del punto de inicio para la sección de pastel después de llamar al método Chart.Calculate(). Se aplica al gráfico de rosquilla.

```csharp
public float InnerArcStartPointYPx { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcStartPointYPxDemo
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
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular el gráfico para asegurar que las propiedades estén pobladas
            chart.Calculate();

            // Obtener el primer punto del gráfico
            ChartPoint point = chart.NSeries[0].Points[0];

            // Muestra el valor de InnerArcStartPointYPx
            Console.WriteLine("InnerArcStartPointYPx: " + point.InnerArcStartPointYPx);

            // Nota: InnerArcStartPointYPx es de solo lectura, por lo que no podemos establecerlo directamente
            // Para cambiar la posición, necesitamos ajustar el tamaño del agujero del donut
            chart.NSeries[0].DoughnutHoleSize = 50; // Percentage of the chart size

            // Recalcula el gráfico para actualizar las propiedades
            chart.Calculate();

            // Muestra el nuevo valor de InnerArcStartPointYPx después de cambiar el tamaño del agujero
            Console.WriteLine("New InnerArcStartPointYPx after changing hole size: " + point.InnerArcStartPointYPx);

            // Guarda el libro de trabajo
            workbook.Save("ChartPointPropertyInnerArcStartPointYPxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


