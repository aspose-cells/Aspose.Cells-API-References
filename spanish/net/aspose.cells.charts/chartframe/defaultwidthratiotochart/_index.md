---
title: "ChartFrame.DefaultWidthRatioToChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Representa el ancho de la posición predeterminada en unidades de Fracción del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartframe/defaultwidthratiotochart/
---
## ChartFrame.DefaultWidthRatioToChart property

Representa el ancho de la posición predeterminada en unidades de fracción del área del gráfico.

```csharp
public double DefaultWidthRatioToChart { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultWidthRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder al título del gráfico que es un ChartFrame
            ChartFrame chartTitle = chart.Title;

            // Mostrar el valor actual de DefaultWidthRatioToChart
            Console.WriteLine("Current DefaultWidthRatioToChart value: " + chartTitle.DefaultWidthRatioToChart);

            // Nota: DefaultWidthRatioToChart es de solo lectura, por lo que no podemos establecerlo
            // En su lugar, demostraremos su relación con la proporción de ancho real
            Console.WriteLine("Current WidthRatioToChart: " + chartTitle.WidthRatioToChart);

            // Cambiar la proporción de ancho para demostrar su efecto
            chartTitle.WidthRatioToChart = 0.5;
            Console.WriteLine("After setting WidthRatioToChart to 0.5, DefaultWidthRatioToChart remains: " + chartTitle.DefaultWidthRatioToChart);

            // Guarda el libro de trabajo
            workbook.Save("ChartFramePropertyDefaultWidthRatioToChartDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


