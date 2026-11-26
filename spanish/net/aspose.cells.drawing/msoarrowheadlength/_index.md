---
title: "Enum MsoArrowheadLength"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Drawing.MsoArrowheadLength. Enumera el ancho del extremo de línea del borde de la forma"
type: docs
url: /es/net/aspose.cells.drawing/msoarrowheadlength/
---
## MsoArrowheadLength enumeration

Enumera el ancho del extremo de línea del borde de la forma.

```csharp
public enum MsoArrowheadLength
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Short | `0` | Longitud corta del extremo de línea |
| Medium | `1` | Longitud media del extremo de línea |
| Long | `2` | Longitud larga del extremo de línea |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoArrowheadLengthDemo
    {
        public static void MsoArrowheadLengthExample()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer el rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", true);

            // Crear una forma de línea para el gráfico
            Line line = chart.Line;

            // Establecer las longitudes de la punta de flecha
            line.BeginArrowLength = MsoArrowheadLength.Medium;
            line.EndArrowLength = MsoArrowheadLength.Long;

            // Salida de las longitudes de la punta de flecha
            Console.WriteLine("Begin Arrowhead Length: " + line.BeginArrowLength);
            Console.WriteLine("End Arrowhead Length: " + line.EndArrowLength);

            // Guarda el libro de trabajo
            workbook.Save("MsoArrowheadLengthExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


