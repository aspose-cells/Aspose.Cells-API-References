---
title: "PlotArea.HeightRatioToChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PlotArea. Obtiene o establece la altura del cuadro delimitador del área de trazado en unidades de la proporción del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/plotarea/heightratiotochart/
---
## PlotArea.HeightRatioToChart property

Obtiene o establece la altura del cuadro delimitador del área de trazado en unidades de la proporción del área del gráfico.

```csharp
public override double HeightRatioToChart { get; set; }
```

### Observaciones

El cuadro delimitador del área de trazado incluye el área de trazado, las marcas de graduación (etiquetas de graduación) y un pequeño borde alrededor de las marcas de graduación. Si el valor no fue creado por MS Excel, por favor llame al método Chart.Calculate() antes de llamar a este método.

El **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** y **HeightRatioToChart** de **PlotArea** representan el cuadro delimitador del área de trazado que incluye el área de trazado, las marcas de graduación (etiquetas de marcas) y un pequeño borde alrededor de las marcas de graduación. Si desea obtener el tamaño real del área de trazado, debe llamar a las propiedades **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** y **InnerHeightRatioToChart**.

Para Excel 2007 o posterior, el valor predeterminado es cero. Debe obtener el valor después de llamar a Chart.Calculate().

HeightPixel = HeightRatioToChart * chart.ChartObject.Width. Nota: Cuando se establece HeightRatioToChart, la propiedad IsInnerMode se establecerá automáticamente en false.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyHeightRatioToChartDemo
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
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtener el área de trazado del gráfico
            PlotArea plotArea = chart.PlotArea;

            // Mostrar la proporción de altura actual
            Console.WriteLine("Current HeightRatioToChart value: " + plotArea.HeightRatioToChart);

            // Establecer una nueva proporción de altura (0.7 significa 70% de la altura del área del gráfico)
            plotArea.HeightRatioToChart = 0.7;

            // Mostrar la nueva proporción de altura
            Console.WriteLine("New HeightRatioToChart value: " + plotArea.HeightRatioToChart);

            // Guardar el libro de trabajo para ver el efecto
            workbook.Save("PlotAreaHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


