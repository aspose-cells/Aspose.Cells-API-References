---
title: "Axis.TickMarkSpacing"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Devuelve o establece el número de categorías o series entre marcas de graduación. Se aplica solo a ejes de categoría y de series"
type: docs
url: /es/net/aspose.cells.charts/axis/tickmarkspacing/
---
## Axis.TickMarkSpacing property

Devuelve o establece el número de categorías o series entre marcas de graduación. Se aplica solo a los ejes de categorías y series.

```csharp
public int TickMarkSpacing { get; set; }
```

### Observaciones

El número debe estar entre 1 y 31999.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTickMarkSpacingDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configurar el eje de valores con TickMarkSpacing
            Axis valueAxis = chart.ValueAxis;
            valueAxis.MinValue = 0;
            valueAxis.MaxValue = 200;
            valueAxis.MajorUnit = 25;
            valueAxis.MinorUnit = 5;
            valueAxis.TickMarkSpacing = 2; // Setting tick mark spacing
            
            // Configurar el eje de categoría con TickMarkSpacing
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.TickMarkSpacing = 1; // Setting tick mark spacing

            workbook.Save("AxisTickMarkSpacingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


