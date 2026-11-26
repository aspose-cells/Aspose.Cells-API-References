---
title: "Axis.MinorTickMark"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa el tipo de marca de graduación menor para el eje especificado"
type: docs
url: /es/net/aspose.cells.charts/axis/minortickmark/
---
## Axis.MinorTickMark property

Representa el tipo de marca de graduación menor para el eje especificado.

```csharp
public TickMarkType MinorTickMark { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinorTickMarkDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos de ejemplo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Crear gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configurar propiedades del eje
            Axis valueAxis = chart.ValueAxis;
            valueAxis.MinorTickMark = TickMarkType.Inside;
            valueAxis.MajorTickMark = TickMarkType.Cross;
            valueAxis.MinValue = 0;
            valueAxis.MaxValue = 200;
            valueAxis.MajorUnit = 25;

            workbook.Save("AxisMinorTickMarkDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TickMarkType](../../tickmarktype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


