---
title: "Klasse DropBars"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.DropBars Klasse. Stellt die Auf‑ und Ab‑Balken in einem Diagramm dar."
type: docs
url: /de/net/aspose.cells.charts/dropbars/
---
## DropBars class

Stellt die Aufwärts‑ und Abwärtsbalken in einem Diagramm dar.

```csharp
public class DropBars
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Area](../../aspose.cells.charts/dropbars/area/) { get; } | Ruft das [`Area`](./area/) ab. |
| [Border](../../aspose.cells.charts/dropbars/border/) { get; } | Ruft die Rahmen‑[`Line`](../../aspose.cells.drawing/line/) ab. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DropBarsDemo
    {
        public static void DropBarsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Füge NSeries (Diagrammdatenquelle) zum Diagramm hinzu, das vom Feld "A1" bis "B3" reicht.
            chart.NSeries.Add("A1:B3", true);

            // Aktivieren Sie Auf‑ und Ab‑Balken
            chart.NSeries[0].HasUpDownBars = true;

            // Greifen Sie auf das DropBars‑Objekt zu
            DropBars upBars = chart.NSeries[0].UpBars;
            DropBars downBars = chart.NSeries[0].DownBars;

            // Passen Sie das Aussehen der Auf‑Balken an
            upBars.Border.Color = Color.Green;
            upBars.Area.ForegroundColor = Color.LightGreen;

            // Passen Sie das Aussehen der Ab‑Balken an
            downBars.Border.Color = Color.Red;
            downBars.Area.ForegroundColor = Color.LightCoral;

            // Speichere die Arbeitsmappe
            workbook.Save("DropBarsExample.xlsx");
            workbook.Save("DropBarsExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


