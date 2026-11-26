---
title: "Axis.IsAutoTickLabelSpacing"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Indica si el espaciado de las etiquetas de marcas es automático"
type: docs
url: /es/net/aspose.cells.charts/axis/isautoticklabelspacing/
---
## Axis.IsAutoTickLabelSpacing property

Indica si el espaciado de la etiqueta de marca de graduación es automático

```csharp
public bool IsAutoTickLabelSpacing { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutoTickLabelSpacingDemo
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

            // Configurar eje de valores
            Axis valueAxis = chart.ValueAxis;
            valueAxis.IsAutoTickLabelSpacing = true; // Core property demonstration
            
            // Configurar eje de categorías
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.IsAutoTickLabelSpacing = false; // Core property demonstration
            categoryAxis.TickLabelSpacing = 2;

            workbook.Save("AxisPropertyIsAutoTickLabelSpacingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


