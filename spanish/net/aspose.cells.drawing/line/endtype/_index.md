---
title: "Line.EndType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Line. Especifica una punta de flecha para el final de una línea"
type: docs
url: /es/net/aspose.cells.drawing/line/endtype/
---
## Line.EndType property

Especifica una punta de flecha para el final de una línea.

```csharp
public MsoArrowheadStyle EndType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyEndTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // Agregue una línea de tendencia y establezca EndType
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Aspose.Cells.Charts.Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.EndType = MsoArrowheadStyle.Arrow;
            trendline.EndArrowLength = MsoArrowheadLength.Medium;
            trendline.EndArrowWidth = MsoArrowheadWidth.Medium;

            workbook.Save("LineEndTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


