---
title: "Enumeración LineJoinType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.LineJoinType. Representa los estilos de unión de una línea"
type: docs
url: /es/net/aspose.cells.drawing/linejointype/
---
## LineJoinType enumeration

Representa los estilos de unión de una línea.

```csharp
public enum LineJoinType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Round | `0` | Unión redondeada |
| Bevel | `1` | Unión biselada |
| Miter | `2` | Unión a inglete |
| None | `3` | Sin unión |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LineJoinTypeDemo
    {
        public static void LineJoinTypeExample()
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

            // Acceder al eje de valores principal
            Axis valueAxis = chart.ValueAxis;

            // Acceder al formato de línea de las cuadrículas principales
            Line majorGridLines = valueAxis.MajorGridLines;

            // Establecer el tipo de unión de la línea
            majorGridLines.JoinType = LineJoinType.Round;

            // Mostrar el tipo de unión
            Console.WriteLine("Line Join Type: " + majorGridLines.JoinType);

            // Guarda el libro de trabajo
            workbook.Save("LineJoinTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


