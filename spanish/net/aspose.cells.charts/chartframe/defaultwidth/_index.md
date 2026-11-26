---
title: "ChartFrame.DefaultWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Representa el ancho de la posición predeterminada en unidades de 1/4000 del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartframe/defaultwidth/
---
## ChartFrame.DefaultWidth property

Representa el ancho de la posición predeterminada en unidades de 1/4000 del área del gráfico.

```csharp
[Obsolete("Use ChartFrame.DefaultWidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int DefaultWidth { get; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. Por favor use la propiedad ChartFrame.DefaultWidthRatioToChart, en su lugar. DefaultWidth = (int)(DefaultWidthRatioToChart * 4000); Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultWidthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            
            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Acceder al título del gráfico (que hereda de ChartFrame)
            Title title = chart.Title;
            
            // Mostrar el ancho predeterminado del marco del gráfico (título en este caso)
            Console.WriteLine("DefaultWidth of chart title: " + title.DefaultWidth);
            
            // Nota: DefaultWidth es de solo lectura, por lo que no podemos establecerlo
            // Solo podemos leerlo para comprender las dimensiones predeterminadas
            
            // Demostrar cómo esta propiedad afecta al gráfico
            Console.WriteLine("IsDefaultPosBeSet: " + title.IsDefaultPosBeSet);
            Console.WriteLine("DefaultWidthRatioToChart: " + title.DefaultWidthRatioToChart);
            
            // Guarda el libro de trabajo
            workbook.Save("ChartFrameDefaultWidthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


