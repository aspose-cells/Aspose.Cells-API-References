---
title: "PlotArea.IsAutomaticSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PlotArea. Indica si el área de trazado se dimensiona automáticamente"
type: docs
url: /es/net/aspose.cells.charts/plotarea/isautomaticsize/
---
## PlotArea.IsAutomaticSize property

Indica si el área de trazado tiene un tamaño automático.

```csharp
public override bool IsAutomaticSize { get; set; }
```

### Observaciones

NOTA: Cuando IsAutomaticSize se establece en True, los valores que usted establezca manualmente para Width y Height se deshabilitarán.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyIsAutomaticSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configurar el área de trazado
            PlotArea plotArea = chart.PlotArea;
            plotArea.IsAutomaticSize = false; // Disable automatic sizing
            plotArea.Width = 3000;
            plotArea.Height = 2000;

            workbook.Save("PlotAreaIsAutomaticSizeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


