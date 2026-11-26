---
title: "ChartPoint.InnerArcStartPointXPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartPoint. Obtiene la coordenada x del punto inicial para la sección de pastel después de llamar al método Chart.Calculate. Se aplica al gráfico Doughnut"
type: docs
url: /es/net/aspose.cells.charts/chartpoint/innerarcstartpointxpx/
---
## ChartPoint.InnerArcStartPointXPx property

Obtiene la coordenada x del punto inicial de la sección de pastel después de llamar al método Chart.Calculate(). Se aplica al gráfico de dona.

```csharp
public float InnerArcStartPointXPx { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyInnerArcStartPointXPxDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de anillo
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular el gráfico para obtener las propiedades de forma
            chart.Calculate();

            // Obtener el primer punto del gráfico
            ChartPoint point = chart.NSeries[0].Points[0];

            // Mostrar el valor de InnerArcStartPointXPx
            Console.WriteLine("InnerArcStartPointXPx: " + point.InnerArcStartPointXPx);

            // Nota: InnerArcStartPointXPx es de solo lectura, por lo que no podemos establecerlo directamente
            // Para cambiar la posición, necesitaríamos modificar el tamaño del gráfico o el tamaño del agujero del anillo

            // Guarda el libro de trabajo
            workbook.Save("ChartPointPropertyInnerArcStartPointXPxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


