---
title: "Enumeración MsoArrowheadWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.MsoArrowheadWidth. Enumera el ancho del extremo de línea del borde de la forma"
type: docs
url: /es/net/aspose.cells.drawing/msoarrowheadwidth/
---
## MsoArrowheadWidth enumeration

Enumera el ancho del extremo de línea del borde de la forma.

```csharp
public enum MsoArrowheadWidth
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Narrow | `0` | Ancho corto del extremo de línea. |
| Medium | `1` | Ancho medio del extremo de línea. |
| Wide | `2` | Ancho amplio del extremo de línea. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class MsoArrowheadWidthDemo
    {
        public static void MsoArrowheadWidthExample()
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

            // Crear una forma de línea para el gráfico
            Line line = chart.Line;

            // Establecer los estilos y anchos de la punta de flecha
            line.BeginType = MsoArrowheadStyle.Arrow;
            line.BeginArrowWidth = MsoArrowheadWidth.Wide;
            line.EndType = MsoArrowheadStyle.Arrow;
            line.EndArrowWidth = MsoArrowheadWidth.Narrow;

            // Mostrar los estilos y anchos de la punta de flecha
            Console.WriteLine("Begin Arrowhead Width: " + line.BeginArrowWidth);
            Console.WriteLine("End Arrowhead Width: " + line.EndArrowWidth);

            // Guarda el libro de trabajo
            workbook.Save("MsoArrowheadWidthExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


