---
title: "PlotArea.X"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PlotArea. Obtiene o establece la coordenada x de la esquina superior izquierda del cuadro delimitador del área de trazado en unidades de 1/4000 del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/plotarea/x/
---
## PlotArea.X property

Obtiene o establece la coordenada x de la esquina superior izquierda del cuadro delimitador del área de trazado en unidades de 1/4000 del área del gráfico.

```csharp
[Obsolete("Use PlotArea.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```

### Observaciones

El cuadro delimitador del área de trazado incluye el área de trazado, las marcas de graduación (etiquetas de graduación) y un pequeño borde alrededor de las marcas de graduación. Si el valor no fue creado por MS Excel, por favor llame al método Chart.Calculate() antes de llamar a este método.

El **X**, **Y**, **Width** y **Height** de **PlotArea** representan el cuadro delimitador del área de trazado que incluye el área de trazado, las marcas de graduación (etiquetas de marcas) y un pequeño borde alrededor de las marcas de graduación. Si desea obtener el tamaño real del área de trazado, debe llamar a las propiedades **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** y **InnerHeightRatioToChart**.

Para Excel 2007 o posterior, el valor predeterminado es cero. Debe obtener el valor después de llamar a Chart.Calculate().

Nota: Cuando se establece X, la propiedad IsInnerMode se establecerá automáticamente en false.

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad PlotArea.XRatioToChart, en su lugar. X = XRatioToChart * 4000. Esta propiedad será eliminada 12 meses después, a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyXDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer propiedades de PlotArea
            chart.PlotArea.X = 100;  // Demonstrate X property usage
            chart.PlotArea.Y = 200;
            chart.PlotArea.Width = 1000;
            chart.PlotArea.Height = 800;

            // Guarda el libro de trabajo
            workbook.Save("PlotAreaPropertyXDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


