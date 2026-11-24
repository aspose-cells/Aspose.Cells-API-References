---
title: "Line.EndArrowWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Linieneigenschaft. Gibt die Breite der Pfeilspitze für das Ende einer Linie an"
type: docs
url: /de/net/aspose.cells.drawing/line/endarrowwidth/
---
## Line.EndArrowWidth property

Gibt die Breite der Pfeilspitze für das Ende einer Linie an.

```csharp
public MsoArrowheadWidth EndArrowWidth { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten für ein Liniendiagramm hinzu
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(6);

            // Ein Liniendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("A1:B3", true);

            // Konfiguriere Linieneigenschaften für die erste Serie
            Series series = chart.NSeries[0];
            series.Border.EndArrowWidth = MsoArrowheadWidth.Wide;
            series.Border.EndType = MsoArrowheadStyle.Arrow;

            // Speichere die Arbeitsmappe
            workbook.Save("LinePropertyEndArrowWidthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


