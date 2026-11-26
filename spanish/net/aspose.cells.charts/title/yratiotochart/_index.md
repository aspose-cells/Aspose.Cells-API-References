---
title: "Title.YRatioToChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Title. Obtiene o establece la coordenada y de la esquina superior izquierda en unidades de fracción del área del gráfico. Y en píxeles  YRatioToChart  Chart.ChartObject.Width"
type: docs
url: /es/net/aspose.cells.charts/title/yratiotochart/
---
## Title.YRatioToChart property

Obtiene o establece la coordenada y de la esquina superior izquierda en unidades de fracción del área del gráfico. Y en píxeles = YRatioToChart * Chart.ChartObject.Width;

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

    public class TitlePropertyYRatioToChartDemo
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

            // Obtenga el título del gráfico
            chart.Title.Text = "Sample Chart Title";
            Title chartTitle = chart.Title;

            // Mostrar el valor actual de YRatioToChart
            Console.WriteLine("Current YRatioToChart value: " + chartTitle.YRatioToChart);

            // Cambiar la propiedad YRatioToChart para mover el título verticalmente
            chartTitle.YRatioToChart = 0.1; // 10% from the top of the chart area
            Console.WriteLine("New YRatioToChart value: " + chartTitle.YRatioToChart);

            // Guarda el libro de trabajo
            workbook.Save("TitlePropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


