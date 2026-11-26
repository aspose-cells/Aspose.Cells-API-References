---
title: "Enumeración GradientDirectionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.GradientDirectionType. Representa todos los tipos de dirección del degradado"
type: docs
url: /es/net/aspose.cells.drawing/gradientdirectiontype/
---
## GradientDirectionType enumeration

Representa todos los tipos de dirección del degradado.

```csharp
public enum GradientDirectionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| FromUpperLeftCorner | `0` | FromUpperLeftCorner |
| FromUpperRightCorner | `1` | FromUpperRightCorner |
| FromLowerLeftCorner | `2` | FromLowerLeftCorner |
| FromLowerRightCorner | `3` | FromLowerRightCorner |
| FromCenter | `4` | FromCenter |
| Unknown | `5` | Desconocido |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientDirectionTypeDemo
    {
        public static void GradientDirectionTypeExample()
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

            // Establece un relleno de degradado de dos colores con una dirección específica
            fillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.DiagonalDown, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Salida del tipo de dirección del gradiente
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Guarda el libro de trabajo
            workbook.Save("GradientDirectionTypeExample.xlsx");
            workbook.Save("GradientDirectionTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


