---
title: "ChartFrame.HeightRatioToChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Obtiene o establece la altura del marco en unidades de la proporción del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartframe/heightratiotochart/
---
## ChartFrame.HeightRatioToChart property

Obtiene o establece la altura del marco en unidades de la proporción del área del gráfico.

```csharp
public virtual double HeightRatioToChart { get; set; }
```

### Observaciones

Este es un valor fraccionario, su rango válido está entre 0-1. ¿Cómo convertir unidades de proporción a píxeles? HeightPixel = HeightRatioToChart * Chart.ChartObject.Height;

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyHeightRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder al título del gráfico (que hereda de ChartFrame)
            chart.Title.Text = "Sample Chart";
            ChartFrame titleFrame = chart.Title;

            // Mostrar el valor actual de HeightRatioToChart
            Console.WriteLine("Current HeightRatioToChart value: " + titleFrame.HeightRatioToChart);

            // Establecer una nueva proporción de altura (0.1 = 10% de la altura del gráfico)
            titleFrame.HeightRatioToChart = 0.1;

            // Demostrar el efecto comparando antes/después
            Console.WriteLine("Title height reduced to 10% of chart height");

            // Guardar el resultado
            workbook.Save("PropertyHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


