---
title: "Clase TickLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Charts.TickLabels. Representa las etiquetas de marcas de graduación asociadas a las marcas de graduación en un eje de gráfico"
type: docs
url: /es/net/aspose.cells.charts/ticklabels/
---
## TickLabels class

Representa las etiquetas de marcas asociadas a las marcas de graduación en el eje de un gráfico.

```csharp
public class TickLabels
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AlignmentType](../../aspose.cells.charts/ticklabels/alignmenttype/) { get; set; } | Obtiene y establece la alineación del texto para las etiquetas de marcas en el eje. |
| [AutoScaleFont](../../aspose.cells.charts/ticklabels/autoscalefont/) { get; set; } | True si el texto en el objeto cambia el tamaño de fuente cuando cambia el tamaño del objeto. El valor predeterminado es True. |
| [BackgroundMode](../../aspose.cells.charts/ticklabels/backgroundmode/) { get; set; } | Obtiene y establece el modo de visualización del fondo |
| [DirectionType](../../aspose.cells.charts/ticklabels/directiontype/) { get; set; } | Obtiene y establece la dirección del texto. |
| [DisplayNumberFormat](../../aspose.cells.charts/ticklabels/displaynumberformat/) { get; } | Obtiene y establece el formato numérico de visualización de las etiquetas de marcas. |
| [Font](../../aspose.cells.charts/ticklabels/font/) { get; } | Devuelve un objeto [`Font`](./font/) que representa la fuente del objeto TickLabels especificado. |
| [IsAutomaticRotation](../../aspose.cells.charts/ticklabels/isautomaticrotation/) { get; set; } | Indica si el ángulo de rotación es automático |
| [Number](../../aspose.cells.charts/ticklabels/number/) { get; set; } | Representa el número de formato para el objeto TickLabels. |
| [NumberFormat](../../aspose.cells.charts/ticklabels/numberformat/) { get; set; } | Representa la cadena de formato para el objeto TickLabels. |
| [NumberFormatLinked](../../aspose.cells.charts/ticklabels/numberformatlinked/) { get; set; } | True si el formato numérico está vinculado a las celdas (de modo que el formato numérico cambie en las etiquetas cuando cambie en las celdas). |
| [Offset](../../aspose.cells.charts/ticklabels/offset/) { get; set; } | Obtiene y establece la distancia de las etiquetas al eje de categoría. Esto se aplica solo al eje de categoría (x). |
| [ReadingOrder](../../aspose.cells.charts/ticklabels/readingorder/) { get; set; } | Representa el orden de lectura del texto. |
| [RotationAngle](../../aspose.cells.charts/ticklabels/rotationangle/) { get; set; } | Representa el ángulo de rotación del texto en sentido horario. |
| [TextDirection](../../aspose.cells.charts/ticklabels/textdirection/) { get; set; } | (**Obsolete.**) Representa el orden de lectura del texto. |
| [TickLabelItems](../../aspose.cells.charts/ticklabels/ticklabelitems/) { get; } | Obtiene las etiquetas de marcas de visualización del eje. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelsDemo
    {
        public static void TickLabelsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Agrega NSeries (fuente de datos del gráfico) al gráfico que abarca desde la celda "A1" hasta "B3"
            chart.NSeries.Add("A1:B3", true);

            // Acceder al eje de valores
            Axis valueAxis = chart.ValueAxis;

            // Accede a las etiquetas de marcas del eje de valores
            TickLabels tickLabels = valueAxis.TickLabels;

            // Establece las propiedades de las etiquetas de marcas
            tickLabels.AutoScaleFont = true;
            tickLabels.BackgroundMode = BackgroundMode.Transparent;
            tickLabels.RotationAngle = 45;
            tickLabels.IsAutomaticRotation = false;
            tickLabels.NumberFormat = "0.00";
            tickLabels.Number = 2;
            tickLabels.NumberFormatLinked = true;
            tickLabels.Offset = 100;
            tickLabels.TextDirection = TextDirectionType.LeftToRight;
            tickLabels.ReadingOrder = TextDirectionType.LeftToRight;
            tickLabels.DirectionType = ChartTextDirectionType.Horizontal;
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // Guarda el libro de trabajo
            workbook.Save("TickLabelsExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


