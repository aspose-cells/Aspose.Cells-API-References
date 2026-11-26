---
title: "ChartArea.HeightRatioToChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartArea. Obtiene o establece el desplazamiento vertical desde la fila de su esquina inferior derecha en unidades de proporción del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartarea/heightratiotochart/
---
## ChartArea.HeightRatioToChart property

Obtiene o establece el desplazamiento vertical desde la fila de su esquina inferior derecha, en unidades de proporción del área del gráfico.

```csharp
public override double HeightRatioToChart { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartAreaPropertyHeightRatioToChartDemo
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
            chart.SetChartDataRange("A1:B4", true);

            // Acceder al área del gráfico
            ChartArea chartArea = chart.ChartArea;

            // Mostrar el valor actual de HeightRatioToChart
            Console.WriteLine("Current HeightRatioToChart value: " + chartArea.HeightRatioToChart);

            // Establecer un nuevo valor para HeightRatioToChart (0.5 = 50% de la altura del gráfico)
            chartArea.HeightRatioToChart = 0.5;
            Console.WriteLine("New HeightRatioToChart value: " + chartArea.HeightRatioToChart);

            // Establecer un nuevo valor para WidthRatioToChart para demostrar el efecto combinado
            chartArea.WidthRatioToChart = 0.8;

            // Guarda el libro de trabajo para ver los cambios
            workbook.Save("ChartAreaPropertyHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


