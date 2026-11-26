---
title: "ChartFrame.DefaultYRatioToChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ChartFrame. Representa la y de la posición predeterminada en unidades de la fracción del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartframe/defaultyratiotochart/
---
## ChartFrame.DefaultYRatioToChart property

Representa la y de la posición predeterminada en unidades de la fracción del área del gráfico.

```csharp
public double DefaultYRatioToChart { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultYRatioToChartDemo
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
            
            // Agregar un gráfico y obtener su marco del gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);
            
            // Obtener el marco del gráfico (título en este caso)
            ChartFrame chartFrame = chart.Title;
            
            // Mostrar el valor actual de DefaultYRatioToChart
            Console.WriteLine("Current DefaultYRatioToChart value: " + chartFrame.DefaultYRatioToChart);
            
            // Demostrar cómo cambiar YRatioToChart afecta la posición (ya que DefaultYRatioToChart es de solo lectura)
            Console.WriteLine("Current YRatioToChart value: " + chartFrame.YRatioToChart);
            chartFrame.YRatioToChart = 0.1; // Move title up
            Console.WriteLine("New YRatioToChart value: " + chartFrame.YRatioToChart);
            
            // Guardar el resultado
            workbook.Save("PropertyDefaultYRatioToChartDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


