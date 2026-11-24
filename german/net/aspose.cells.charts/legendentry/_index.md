---
title: "Klasse LegendEntry"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.LegendEntry Klasse. Stellt einen Legendeneintrag in einer Diagrammlegende dar."
type: docs
url: /de/net/aspose.cells.charts/legendentry/
---
## LegendEntry class

Stellt einen Legendeneintrag in einer Diagrammlegende dar.

```csharp
public class LegendEntry
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/legendentry/autoscalefont/) { get; set; } | True, wenn der Text im Objekt die Schriftgröße ändert, wenn die Objektgröße geändert wird. Der Standardwert ist True. |
| [Background](../../aspose.cells.charts/legendentry/background/) { get; set; } | (**Obsolete.**) Liest und setzt den Anzeigemodus des Hintergrunds. |
| [BackgroundMode](../../aspose.cells.charts/legendentry/backgroundmode/) { get; set; } | Liest und setzt den Anzeigemodus des Hintergrunds |
| [Font](../../aspose.cells.charts/legendentry/font/) { get; } | Ruft ein [`Font`](./font/) Objekt des angegebenen ChartFrame-Objekts ab. |
| [IsDeleted](../../aspose.cells.charts/legendentry/isdeleted/) { get; set; } | Liest und setzt, ob der Legendeneintrag gelöscht ist. |
| [IsTextNoFill](../../aspose.cells.charts/legendentry/istextnofill/) { get; set; } | Liest oder setzt keine Füllung des Textes. |
| virtual [TextFont](../../aspose.cells.charts/legendentry/textfont/) { get; } | (**Obsolete.**) Ruft ein [`Font`](./font/) Objekt des angegebenen LegendEntry-Objekts ab. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendEntryDemo
    {
        public static void LegendEntryExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Füge NSeries (Diagrammdatenquelle) zum Diagramm hinzu, das von Zelle "A1" bis "B4" reicht.
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Greife auf den Legendeneintrag der ersten Serie zu.
            LegendEntry legendEntry = chart.NSeries[0].LegendEntry;

            // Setze Eigenschaften des Legendeneintrags
            legendEntry.IsDeleted = false;
            legendEntry.IsTextNoFill = false;
            legendEntry.AutoScaleFont = true;
            legendEntry.Background = BackgroundMode.Transparent;
            legendEntry.BackgroundMode = BackgroundMode.Opaque;

            // Greife auf die Schriftart des Legendeneintrags zu und ändere sie.
            Font font = legendEntry.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            font.Color = System.Drawing.Color.Blue;

            // Speichere die Arbeitsmappe
            workbook.Save("LegendEntryExample.xlsx");
            workbook.Save("LegendEntryExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


