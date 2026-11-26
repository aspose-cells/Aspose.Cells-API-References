---
title: "ChartArea.YRatioToChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartArea. Obtiene o establece el desplazamiento vertical desde la fila de su esquina superior izquierda en unidades de proporción del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartarea/yratiotochart/
---
## ChartArea.YRatioToChart property

Obtiene o recupera el desplazamiento vertical desde la fila de su esquina superior izquierda, en unidades de proporción del área del gráfico.

```csharp
public override double YRatioToChart { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartAreaPropertyYRatioToChartDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder al área del gráfico
            ChartArea chartArea = chart.ChartArea;

            // Mostrar el valor actual de YRatioToChart
            Console.WriteLine("Current YRatioToChart value: " + chartArea.YRatioToChart);

            // Cambiar la propiedad YRatioToChart (0.0 a 1.0 representa del 0% al 100% del área del gráfico)
            chartArea.YRatioToChart = 0.2; // Move chart area down by 20% of chart height

            // Mostrar el nuevo valor de YRatioToChart
            Console.WriteLine("New YRatioToChart value: " + chartArea.YRatioToChart);

            // Guardar el libro de trabajo para ver el efecto
            workbook.Save("ChartAreaPropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


