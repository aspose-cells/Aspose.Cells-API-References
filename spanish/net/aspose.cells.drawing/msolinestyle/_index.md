---
title: "Enum MsoLineStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.MsoLineStyle. Representa el estilo de las líneas de dibujo"
type: docs
url: /es/net/aspose.cells.drawing/msolinestyle/
---
## MsoLineStyle enumeration

Representa el estilo de líneas de dibujo.

```csharp
public enum MsoLineStyle
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Single | `0` | Línea única (de ancho lineWidth) |
| ThickBetweenThin | `1` | Tres líneas, delgada, gruesa, delgada |
| ThinThick | `2` | Líneas dobles, una delgada, una gruesa |
| ThickThin | `3` | Líneas dobles, una gruesa, una delgada |
| ThinThin | `4` | Líneas dobles de ancho igual |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineStyleDemo
    {
        public static void MsoLineStyleExample()
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

            // Establecer el estilo de línea para el eje de categoría principal
            Line axisLine = categoryAxis.AxisLine;
            axisLine.CompoundType = MsoLineStyle.ThickBetweenThin;
            axisLine.Color = Color.Blue;
            axisLine.WeightPt = 2.0;

            // Salida del estilo de línea
            Console.WriteLine("Axis Line Style: " + axisLine.CompoundType);
            Console.WriteLine("Axis Line Color: " + axisLine.Color);
            Console.WriteLine("Axis Line Weight: " + axisLine.WeightPt);

            // Guarda el libro de trabajo
            workbook.Save("MsoLineStyleExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


