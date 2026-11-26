---
title: "LegendEntry.BackgroundMode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LegendEntry. Obtiene y establece el modo de visualización del fondo"
type: docs
url: /es/net/aspose.cells.charts/legendentry/backgroundmode/
---
## LegendEntry.BackgroundMode property

Obtiene y establece el modo de visualización del fondo

```csharp
public BackgroundMode BackgroundMode { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyBackgroundModeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");

            // Crear gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B2", true);
            chart.NSeries.CategoryData = "C1:C2";

            // Configurar entrada de leyenda
            LegendEntry legendEntry = chart.NSeries[0].LegendEntry;
            legendEntry.BackgroundMode = BackgroundMode.Opaque;
            legendEntry.Font.Color = System.Drawing.Color.Blue;

            workbook.Save("LegendEntryBackgroundModeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [BackgroundMode](../../backgroundmode/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


