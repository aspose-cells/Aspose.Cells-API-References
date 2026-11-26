---
title: "PlotArea.InnerWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PlotArea. Obtiene o establece el ancho del área del gráfico en unidades de 1/4000 del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/plotarea/innerwidth/
---
## PlotArea.InnerWidth property

Obtiene o establece el ancho del área del gráfico en unidades de 1/4000 del área del gráfico.

```csharp
[Obsolete("Use PlotArea.InnerWidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int InnerWidth { get; set; }
```

### Observaciones

El cuadro delimitador del área de trazado incluye el área de trazado, las marcas de graduación (etiquetas de graduación) y un pequeño borde alrededor de las marcas de graduación. Si el valor no fue creado por MS Excel, por favor llame al método Chart.Calculate() antes de llamar a este método.

El **X**, **Y**, **Width** y **Height** de **PlotArea** representan el cuadro delimitador del área de trazado que incluye el área de trazado, las marcas de graduación (etiquetas de marcas) y un pequeño borde alrededor de las marcas de graduación. Si desea obtener el tamaño real del área de trazado, debe llamar a las propiedades **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** y **InnerHeightRatioToChart**.

Para Excel 2007 o posterior, el valor predeterminado es cero. Debe obtener el valor después de llamar a Chart.Calculate().

Nota: Cuando se establece InnerWidth, la propiedad IsInnerMode se establecerá automáticamente en True.

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad PlotArea.InnerWidthRatioToChart, en su lugar. InnerWidth = InnerWidthRatioToChart * 4000; Esta propiedad será eliminada 12 meses después, a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyInnerWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Establecer datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configurar el área de trazado
            Aspose.Cells.Charts.PlotArea plotArea = chart.PlotArea;
            plotArea.InnerWidth = 2800; // Main demonstration of InnerWidth property
            plotArea.InnerHeight = 1800;
            plotArea.IsInnerMode = true;

            workbook.Save("PlotAreaInnerWidthDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


