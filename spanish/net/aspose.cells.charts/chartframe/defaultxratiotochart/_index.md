---
title: "ChartFrame.DefaultXRatioToChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Representa la x de la posición predeterminada en unidades de Fracción del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartframe/defaultxratiotochart/
---
## ChartFrame.DefaultXRatioToChart property

Representa x de la posición predeterminada en unidades de fracción del área del gráfico.

```csharp
public double DefaultXRatioToChart { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultXRatioToChartDemo
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

            // Obtener el marco del título del gráfico
            ChartFrame titleFrame = chart.Title;

            // Mostrar el valor actual de DefaultXRatioToChart
            Console.WriteLine("Default X Ratio To Chart (Title): " + titleFrame.DefaultXRatioToChart);

            // Crear un cuadro de texto en el gráfico
            Aspose.Cells.Drawing.TextBox textBox = chart.Shapes.AddTextBoxInChart(50, 50, 200, 100);
            
            // Obtener las propiedades de forma del cuadro de texto en lugar de intentar acceder a ChartFrame directamente
            Console.WriteLine("Default X Ratio To Chart (TextBox): " + titleFrame.DefaultXRatioToChart);

            // Demostrar cómo estas proporciones predeterminadas afectan la posición
            Console.WriteLine("Title X Position (Ratio): " + titleFrame.XRatioToChart);
            Console.WriteLine("TextBox X Position (Ratio): " + titleFrame.XRatioToChart);

            // Guarda el libro de trabajo
            workbook.Save("ChartFrameDefaultXRatioToChartDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


