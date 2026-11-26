---
title: "ChartFrame.YRatioToChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Obtiene o establece la coordenada y de la esquina superior izquierda en unidades de la proporción del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartframe/yratiotochart/
---
## ChartFrame.YRatioToChart property

Obtiene o establece la coordenada y de la esquina superior izquierda en unidades de la proporción del área del gráfico.

```csharp
public virtual double YRatioToChart { get; set; }
```

### Observaciones

Este es un valor fraccionario, su rango válido está entre 0-1. ¿Cómo convertir unidades de proporción a píxeles? YPixel = YRatioToChart * Chart.ChartObject.Height;

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyYRatioToChartDemo
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
            
            // Acceder al título del gráfico que hereda de ChartFrame
            chart.Title.Text = "Sample Chart";
            
            // Mostrar el valor actual de YRatioToChart
            Console.WriteLine("Current Title YRatioToChart value: " + chart.Title.YRatioToChart);
            
            // Cambiar la posición Y del título relativa al área del gráfico
            chart.Title.YRatioToChart = 0.1; // 10% from top of chart area
            
            // Mostrar el nuevo valor de YRatioToChart
            Console.WriteLine("New Title YRatioToChart value: " + chart.Title.YRatioToChart);
            
            // Acceder a la leyenda que también hereda de ChartFrame
            chart.Legend.Position = LegendPositionType.Top;
            
            // Mostrar el valor actual de YRatioToChart para la leyenda
            Console.WriteLine("Current Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
            
            // Cambiar la posición Y de la leyenda relativa al área del gráfico
            chart.Legend.YRatioToChart = 0.15; // 15% from top of chart area
            
            // Mostrar el nuevo valor de YRatioToChart para la leyenda
            Console.WriteLine("New Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
            
            // Guarda el libro de trabajo
            workbook.Save("ChartFramePropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


