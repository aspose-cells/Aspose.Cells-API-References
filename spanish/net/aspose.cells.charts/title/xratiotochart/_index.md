---
title: "Title.XRatioToChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Title. Obtiene o establece la coordenada x de la esquina superior izquierda en unidades de fracción del área del gráfico. X en píxeles  XRatioToChart  Chart.ChartObject.Width"
type: docs
url: /es/net/aspose.cells.charts/title/xratiotochart/
---
## Title.XRatioToChart property

Obtiene o establece la coordenada x de la esquina superior izquierda en unidades de fracción del área del gráfico. X en píxeles = XRatioToChart * Chart.ChartObject.Width;

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

    public class TitlePropertyXRatioToChartDemo
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

            // Establezca la fuente de datos para el gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtenga el título del gráfico
            chart.Title.Text = "Sample Chart Title";
            Title title = chart.Title;

            // Muestre el valor actual de XRatioToChart
            Console.WriteLine("Current XRatioToChart value: " + title.XRatioToChart);

            // Cambie el valor de XRatioToChart para mover el título horizontalmente
            title.XRatioToChart = 0.25; // 25% from the left of the chart area
            Console.WriteLine("New XRatioToChart value: " + title.XRatioToChart);

            // Guarda el libro de trabajo
            workbook.Save("TitlePropertyXRatioToChartDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


