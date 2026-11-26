---
title: "Enumeración MsoLineDashStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.MsoLineDashStyle. Representa el estilo de líneas de guiones dibujadas"
type: docs
url: /es/net/aspose.cells.drawing/msolinedashstyle/
---
## MsoLineDashStyle enumeration

Representa el estilo de líneas de dibujo con guiones.

```csharp
public enum MsoLineDashStyle
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Dash | `0` | Representa una línea de guiones. |
| DashDot | `1` | Representa una línea de guión-punto. |
| DashDotDot | `2` | Representa una línea guión-punto-punto. |
| DashLongDash | `3` | Representa una línea de guión largo-corto. |
| DashLongDashDot | `4` | Representa una línea de guión largo-corto-punto. |
| RoundDot | `5` | Representa una línea de punto redondo. |
| Solid | `6` | Representa una línea continua. |
| SquareDot | `7` | Representa una línea de punto cuadrado. |
| Custom | `8` | Estilo de guión personalizado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineDashStyleDemo
    {
        public static void MsoLineDashStyleExample()
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

            // Establecer el estilo de guión de las líneas de cuadrícula principales
            categoryAxis.MajorGridLines.DashType = MsoLineDashStyle.DashDot;

            // Establecer el estilo de guión de las líneas de cuadrícula secundarias
            categoryAxis.MinorGridLines.DashType = MsoLineDashStyle.DashLongDashDot;

            // Guarda el libro de trabajo
            workbook.Save("MsoLineDashStyleExample.xlsx");

            // Genere la salida de los resultados
            Console.WriteLine("Chart with custom dash styles for gridlines created successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


