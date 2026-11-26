---
title: "Enumeración TickMarkType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.TickMarkType enum. Representa el tipo de marca de graduación para el eje especificado."
type: docs
url: /es/net/aspose.cells.charts/tickmarktype/
---
## TickMarkType enumeration

Representa el tipo de marca de graduación para el eje especificado.

```csharp
public enum TickMarkType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Cross | `0` | El tipo de marca de graduación es Cruz. |
| Inside | `1` | El tipo de marca de graduación es Dentro. |
| None | `2` | El tipo de marca de graduación es Ninguno. |
| Outside | `3` | El tipo de marca de graduación es Fuera |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickMarkTypeDemo
    {
        public static void TickMarkTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
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

            // Accede al eje de valores del gráfico.
            Axis valueAxis = chart.ValueAxis;

            // Establece el tipo de marca de graduación mayor a Cruz
            valueAxis.MajorTickMark = TickMarkType.Cross;

            // Establece el tipo de marca de graduación menor a Dentro
            valueAxis.MinorTickMark = TickMarkType.Inside;

            // Establecer el valor máximo del eje de valores
            valueAxis.MaxValue = 200;

            // Establecer el valor mínimo del eje de valores
            valueAxis.MinValue = 0;

            // Establecer la unidad principal
            valueAxis.MajorUnit = 25;

            // Guarda el libro de trabajo
            workbook.Save("TickMarkTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


