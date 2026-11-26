---
title: "ChartFrame.XRatioToChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Obtiene o establece la coordenada x de la esquina superior izquierda en unidades de proporción del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartframe/xratiotochart/
---
## ChartFrame.XRatioToChart property

Obtiene o establece la coordenada x de la esquina superior izquierda en unidades de la proporción del área del gráfico.

```csharp
public virtual double XRatioToChart { get; set; }
```

### Observaciones

Este es un valor fraccionario, su rango válido está entre 0-1. ¿Cómo convertir unidades de proporción a píxeles? XPixel = XRatioToChart * Chart.ChartObject.Width;

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyXRatioToChartDemo
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

            // Acceder al título del gráfico que es un ChartFrame
            ChartFrame chartTitle = chart.Title;

            // Muestre el valor actual de XRatioToChart
            Console.WriteLine("Current XRatioToChart value: " + chartTitle.XRatioToChart);

            // Establecer nuevo valor de XRatioToChart (0.5 significa el 50 % del ancho del gráfico desde la izquierda)
            chartTitle.XRatioToChart = 0.5;

            // Mostrar nueva posición
            Console.WriteLine("Title position after change - XRatioToChart: " + chartTitle.XRatioToChart);

            // Guarda el libro de trabajo
            workbook.Save("ChartFrameXRatioToChartDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


