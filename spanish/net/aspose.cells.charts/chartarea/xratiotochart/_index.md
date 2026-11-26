---
title: "ChartArea.XRatioToChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartArea. Obtiene o establece el desplazamiento horizontal desde la columna de su esquina superior izquierda como una razón del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartarea/xratiotochart/
---
## ChartArea.XRatioToChart property

Obtiene o establece el desplazamiento horizontal desde la columna de la esquina superior‑izquierda, como una proporción del área del gráfico.

```csharp
public override double XRatioToChart { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartAreaPropertyXRatioToChartDemo
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

            // Obtenga el área del gráfico
            ChartArea chartArea = chart.ChartArea;

            // Muestre el valor actual de XRatioToChart
            Console.WriteLine("Current XRatioToChart value: " + chartArea.XRatioToChart);

            // Cambie el valor de XRatioToChart para mover el área del gráfico horizontalmente
            chartArea.XRatioToChart = 0.2; // 20% from the left of the chart container

            // Muestre el nuevo valor de XRatioToChart
            Console.WriteLine("New XRatioToChart value: " + chartArea.XRatioToChart);

            // Guarda el libro de trabajo
            workbook.Save("ChartAreaXRatioToChartDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


