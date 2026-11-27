---
title: "Line.EndArrowWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Linjeegenskap. Anger bredden på pilspetsen för slutet av en linje"
type: docs
url: /sv/net/aspose.cells.drawing/line/endarrowwidth/
---
## Line.EndArrowWidth property

Anger bredden på pilspetsen för slutet av en linje.

```csharp
public MsoArrowheadWidth EndArrowWidth { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LinePropertyEndArrowWidthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för linjediagram
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(6);

            // Lägg till ett linjediagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("A1:B3", true);

            // Konfigurera linjeegenskaper för den första serien
            Series series = chart.NSeries[0];
            series.Border.EndArrowWidth = MsoArrowheadWidth.Wide;
            series.Border.EndType = MsoArrowheadStyle.Arrow;

            // Spara arbetsboken
            workbook.Save("LinePropertyEndArrowWidthDemo.xlsx");
        }
    }
}
```

### Se även

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


