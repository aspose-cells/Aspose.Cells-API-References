---
title: "ChartFrame.YPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Obtiene o establece la coordenada y de la esquina superior izquierda en unidades de píxeles"
type: docs
url: /es/net/aspose.cells.charts/chartframe/ypixel/
---
## ChartFrame.YPixel property

Obtiene o establece la coordenada y de la esquina superior izquierda en unidades de píxeles.

```csharp
public virtual int YPixel { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyYPixelDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder al título del gráfico (que hereda de ChartFrame)
            chart.Title.Text = "Sample Chart";
            ChartFrame chartFrame = chart.Title;

            // Mostrar el valor actual de YPixel
            Console.WriteLine("Current YPixel value: " + chartFrame.YPixel);

            // Cambiar la posición YPixel del título del gráfico
            chartFrame.YPixel = 50;
            Console.WriteLine("New YPixel value: " + chartFrame.YPixel);

            // Guarda el libro de trabajo
            workbook.Save("ChartFrameYPixelDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


