---
title: "Enumeración GradientStyleType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.GradientStyleType enum. Representa el estilo de sombreado de degradado"
type: docs
url: /es/net/aspose.cells.drawing/gradientstyletype/
---
## GradientStyleType enumeration

Representa el estilo de sombreado del degradado.

```csharp
public enum GradientStyleType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| DiagonalDown | `0` | Estilo de sombreado diagonal descendente |
| DiagonalUp | `1` | Estilo de sombreado diagonal ascendente |
| FromCenter | `2` | Estilo de sombreado desde el centro |
| FromCorner | `3` | Estilo de sombreado desde la esquina |
| Horizontal | `4` | Estilo de sombreado horizontal |
| Vertical | `5` | Estilo de sombreado vertical |
| Unknown | `6` | Estilo de sombreado desconocido. Solo para el estilo de sombreado (que no corresponde a ningún miembro de GradientStyleType) en el archivo de plantilla. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStyleTypeDemo
    {
        public static void GradientStyleTypeExample()
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

            // Acceder al área de trazado del gráfico
            PlotArea plotArea = chart.PlotArea;

            // Acceder al formato de relleno del área de trazado
            FillFormat fillFormat = plotArea.Area.FillFormat;

            // Establecer un relleno de degradado de dos colores con estilo DiagonalDown
            fillFormat.SetTwoColorGradient(Color.Blue, Color.White, GradientStyleType.DiagonalDown, 1);

            // Mostrar el estilo de degradado utilizado
            Console.WriteLine("Gradient Style: " + fillFormat.GradientStyle);

            // Guarda el libro de trabajo
            workbook.Save("GradientStyleTypeExample.xlsx");
            workbook.Save("GradientStyleTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


