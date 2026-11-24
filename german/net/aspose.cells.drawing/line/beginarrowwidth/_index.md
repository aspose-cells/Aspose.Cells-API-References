---
title: "Line.BeginArrowWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Line property. Gibt die Breite der Pfeilspitze für den Anfang einer Linie an"
type: docs
url: /de/net/aspose.cells.drawing/line/beginarrowwidth/
---
## Line.BeginArrowWidth property

Gibt die Breite der Pfeilspitze für den Anfang einer Linie an.

```csharp
public MsoArrowheadWidth BeginArrowWidth { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyBeginArrowWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Diagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Fügen Sie eine Trendlinie hinzu und setzen Sie die Pfeileigenschaften
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.BeginType = MsoArrowheadStyle.Arrow;
            trendline.BeginArrowWidth = MsoArrowheadWidth.Wide;
            trendline.EndType = MsoArrowheadStyle.Arrow;
            trendline.EndArrowWidth = MsoArrowheadWidth.Narrow;

            workbook.Save("LinePropertyBeginArrowWidthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


