---
title: "ChartFrame.DefaultX"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ChartFrame. Representa la x de la posición predeterminada en unidades de 1/4000 del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartframe/defaultx/
---
## ChartFrame.DefaultX property

Representa la x de la posición predeterminada en unidades de 1/4000 del área del gráfico.

```csharp
[Obsolete("Use ChartFrame.DefaultXRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultX { get; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad ChartFrame.DefaultXRatioToChart, en su lugar. DefaultX = (int)(DefaultXRatioToChart * 4000); Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultXDemo
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
            
            // Mostrar la posición X predeterminada del título del gráfico
            Console.WriteLine("Default X position (1/4000 of chart area): " + chart.Title.DefaultX);
            Console.WriteLine("Default X position (ratio of chart area): " + chart.Title.DefaultXRatioToChart);
            
            // Demostrar cómo la posición predeterminada afecta al gráfico
            Console.WriteLine("Is default position set? " + chart.Title.IsDefaultPosBeSet);
            
            // Cambiar la posición del título usando propiedades de razón (ya que DefaultX es de solo lectura)
            chart.Title.XRatioToChart = 0.2;
            chart.Title.YRatioToChart = 0.05;
            
            // Guarda el libro de trabajo
            workbook.Save("ChartFrameDefaultXDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


