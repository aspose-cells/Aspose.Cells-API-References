---
title: "Line.BeginType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Line property. Gibt eine Pfeilspitze für den Anfang einer Linie an"
type: docs
url: /de/net/aspose.cells.drawing/line/begintype/
---
## Line.BeginType property

Gibt eine Pfeilspitze für den Anfang einer Linie an.

```csharp
public MsoArrowheadStyle BeginType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyBeginTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Ein Liniendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("A1:A3", true);

            // Holen Sie die erste Serie und konfigurieren Sie deren Linieneigenschaften
            Series series = chart.NSeries[0];
            series.Border.BeginType = MsoArrowheadStyle.Arrow;
            series.Border.EndType = MsoArrowheadStyle.ArrowDiamond;
            series.Border.Color = Color.Red;
            series.Border.Weight = WeightType.MediumLine;

            // Speichere die Arbeitsmappe
            workbook.Save("LinePropertyBeginTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


