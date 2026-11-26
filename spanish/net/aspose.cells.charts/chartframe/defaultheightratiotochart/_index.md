---
title: "ChartFrame.DefaultHeightRatioToChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Representa la altura de la posición predeterminada en unidades de la fracción del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartframe/defaultheightratiotochart/
---
## ChartFrame.DefaultHeightRatioToChart property

Representa la altura de la posición predeterminada en unidades de la fracción del área del gráfico.

```csharp
public double DefaultHeightRatioToChart { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultHeightRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder al título del gráfico (que es un ChartFrame)
            ChartFrame chartTitle = chart.Title;

            // Mostrar el valor actual de DefaultHeightRatioToChart
            Console.WriteLine("Current DefaultHeightRatioToChart value: " + chartTitle.DefaultHeightRatioToChart);

            // Demostrar cómo esta propiedad afecta al gráfico comparándola con HeightRatioToChart
            Console.WriteLine("Current HeightRatioToChart value: " + chartTitle.HeightRatioToChart);

            // Cambiar la proporción de altura para ver el efecto
            chartTitle.HeightRatioToChart = 0.1;
            Console.WriteLine("After setting HeightRatioToChart to 0.1: " + chartTitle.HeightRatioToChart);

            // Guarda el libro de trabajo
            workbook.Save("ChartFramePropertyDefaultHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


