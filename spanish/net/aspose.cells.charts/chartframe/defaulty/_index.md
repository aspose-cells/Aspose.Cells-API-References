---
title: "ChartFrame.DefaultY"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Representa la y de la posición predeterminada en unidades de 1/4000 del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartframe/defaulty/
---
## ChartFrame.DefaultY property

Representa la y de la posición predeterminada en unidades de 1/4000 del área del gráfico.

```csharp
[Obsolete("Use ChartFrame.DefaultYRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultY { get; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad ChartFrame.DefaultYRatioToChart, en su lugar. DefaultY = (int)(DefaultYRatioToChart * 4000); Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspree se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultYDemo
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
            
            // Acceder al título del gráfico que hereda de ChartFrame
            chart.Title.Text = "Sample Chart";
            ChartFrame chartFrame = chart.Title;
            
            // Mostrar el valor actual de DefaultY (propiedad de solo lectura)
            Console.WriteLine("DefaultY value (1/4000 of chart area): " + chartFrame.DefaultY);
            Console.WriteLine("DefaultY ratio to chart area: " + chartFrame.DefaultYRatioToChart);
            
            // Demostrar cómo DefaultY afecta la posición comparándola con la posición actual
            Console.WriteLine("Current Y position (ratio): " + chartFrame.YRatioToChart);
            
            // Restablecer la posición a la predeterminada usando SetPositionAuto()
            chartFrame.SetPositionAuto();
            Console.WriteLine("Y position after reset (ratio): " + chartFrame.YRatioToChart);
            
            // Guardar el resultado
            workbook.Save("ChartFramePropertyDefaultYDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


