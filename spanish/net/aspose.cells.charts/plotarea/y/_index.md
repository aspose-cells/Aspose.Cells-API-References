---
title: "PlotArea.Y"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PlotArea. Obtiene o establece la coordenada y de la esquina superior del cuadro delimitador del área de trazado en unidades de 1/4000 del área del gráfico."
type: docs
url: /es/net/aspose.cells.charts/plotarea/y/
---
## PlotArea.Y property

Obtiene o establece la coordenada y de la esquina superior del cuadro delimitador del área de trazado en unidades de 1/4000 del área del gráfico.

```csharp
[Obsolete("Use PlotArea.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Y { get; set; }
```

### Observaciones

El cuadro delimitador del área de trazado incluye el área de trazado, las marcas de graduación (etiquetas de graduación) y un pequeño borde alrededor de las marcas de graduación. Si el valor no fue creado por MS Excel, por favor llame al método Chart.Calculate() antes de llamar a este método.

El **X**, **Y**, **Width** y **Height** de **PlotArea** representan el cuadro delimitador del área de trazado que incluye el área de trazado, las marcas de graduación (etiquetas de marcas) y un pequeño borde alrededor de las marcas de graduación. Si desea obtener el tamaño real del área de trazado, debe llamar a las propiedades **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** y **InnerHeightRatioToChart**.

Para Excel 2007 o posterior, el valor predeterminado es cero. Debe obtener el valor después de llamar a Chart.Calculate().

Nota: Cuando se establece Y, la propiedad IsInnerMode se establecerá automáticamente en false.

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad PlotArea.YRatioToChart, en su lugar. Y = YRatioToChart * 4000. Esta propiedad será eliminada 12 meses después, a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Datos de ejemplo
            sheet.Cells["A1"].PutValue("Category 1");
            sheet.Cells["A2"].PutValue("Category 2");
            sheet.Cells["B1"].PutValue(100);
            sheet.Cells["B2"].PutValue(50);

            // Crear gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Establecer datos del gráfico
            chart.NSeries.Add("B1:B2", false);
            chart.NSeries.CategoryData = "A1:A2";

            // Configurar el área de trazado
            chart.PlotArea.Width = 300;
            chart.PlotArea.Height = 200;
            chart.PlotArea.X = 100;
            chart.PlotArea.Y = 150; // Demonstrating Y property usage

            // Guarda el libro de trabajo
            workbook.Save("PlotAreaPropertyYDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


