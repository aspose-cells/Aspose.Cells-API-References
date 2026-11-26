---
title: "Axis.TickLabelSpacing"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa el número de categorías o series entre las etiquetas de marcas de graduación. Se aplica solo a ejes de categorías y series"
type: docs
url: /es/net/aspose.cells.charts/axis/ticklabelspacing/
---
## Axis.TickLabelSpacing property

Representa el número de categorías o series entre las etiquetas de marcas de graduación. Se aplica solo a los ejes de categorías y series.

```csharp
public int TickLabelSpacing { get; set; }
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
    public class AxisPropertyTickLabelSpacingDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B5"].PutValue(40);

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer datos del gráfico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Configurar espaciado de etiquetas de marcas de graduación del eje
            chart.CategoryAxis.TickLabelSpacing = 2; // Show every 2nd label

            workbook.Save("AxisPropertyTickLabelSpacingDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


