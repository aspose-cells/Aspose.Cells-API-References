---
title: "Enumeración LineType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.LineType enum. Enumera el tipo de borde de Picture o línea de Chart"
type: docs
url: /es/net/aspose.cells.drawing/linetype/
---
## LineType enumeration

Enumera el tipo de borde de [`Picture`](../picture/) o línea de [`Chart`](../../aspose.cells.charts/chart/).

```csharp
public enum LineType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| DarkGray | `6` | Representa una línea gris oscuro. |
| Dash | `1` | Representa una línea de guiones. |
| DashDot | `3` | Representa una línea guión-punto |
| DashDotDot | `4` | Representa una línea guión-punto-punto. |
| Dot | `2` | Representa una línea punteada. |
| LightGray | `8` | Representa una línea gris claro. |
| MediumGray | `7` | Representa una línea gris medio. |
| Solid | `0` | Representa una línea continua. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class LineTypeDemo
    {
        public static void LineTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
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

            // Establecer el rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", true);

            // Acceder al eje de categoría principal
            Axis categoryAxis = chart.CategoryAxis;

            // Establece el tipo de línea para la línea del eje
            categoryAxis.AxisLine.Style = LineType.DashDot;

            // Establece el color de la línea del eje
            categoryAxis.AxisLine.Color = Color.Blue;

            // Acceder al eje de valores principal
            Axis valueAxis = chart.ValueAxis;

            // Establece el tipo de línea para las líneas de cuadrícula principales
            valueAxis.MajorGridLines.Style = LineType.Dot;

            // Establece el color de las líneas de cuadrícula principales
            valueAxis.MajorGridLines.Color = Color.Red;

            // Guarda el libro de trabajo
            workbook.Save("LineTypeExample.xlsx");

            // Genere la salida de los resultados
            Console.WriteLine("Chart created with custom line types for axis and gridlines.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


