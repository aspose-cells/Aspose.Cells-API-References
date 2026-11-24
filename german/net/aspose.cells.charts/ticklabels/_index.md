---
title: "Klasse TickLabels"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.TickLabels Klasse. Stellt die Tickmark‑Beschriftungen dar, die mit den Markierungen auf einer Diagrammachse verbunden sind."
type: docs
url: /de/net/aspose.cells.charts/ticklabels/
---
## TickLabels class

Stellt die Tick-Mark-Labels dar, die mit den Tick-Markierungen auf einer Diagrammachse verbunden sind.

```csharp
public class TickLabels
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AlignmentType](../../aspose.cells.charts/ticklabels/alignmenttype/) { get; set; } | Liest und setzt die Textausrichtung für die Tick‑Beschriftungen auf der Achse. |
| [AutoScaleFont](../../aspose.cells.charts/ticklabels/autoscalefont/) { get; set; } | True, wenn der Text im Objekt die Schriftgröße ändert, wenn die Objektgröße geändert wird. Der Standardwert ist True. |
| [BackgroundMode](../../aspose.cells.charts/ticklabels/backgroundmode/) { get; set; } | Liest und setzt den Anzeigemodus des Hintergrunds |
| [DirectionType](../../aspose.cells.charts/ticklabels/directiontype/) { get; set; } | Liest und legt die Textausrichtung fest. |
| [DisplayNumberFormat](../../aspose.cells.charts/ticklabels/displaynumberformat/) { get; } | Liest und setzt das Anzeige‑Zahlenformat der Tick‑Beschriftungen. |
| [Font](../../aspose.cells.charts/ticklabels/font/) { get; } | Gibt ein [`Font`](./font/)‑Objekt zurück, das die Schriftart des angegebenen TickLabels‑Objekts darstellt. |
| [IsAutomaticRotation](../../aspose.cells.charts/ticklabels/isautomaticrotation/) { get; set; } | Gibt an, ob der Rotationswinkel automatisch ist |
| [Number](../../aspose.cells.charts/ticklabels/number/) { get; set; } | Stellt die Formatnummer für das TickLabels‑Objekt dar. |
| [NumberFormat](../../aspose.cells.charts/ticklabels/numberformat/) { get; set; } | Stellt die Formatzeichenfolge für das TickLabels‑Objekt dar. |
| [NumberFormatLinked](../../aspose.cells.charts/ticklabels/numberformatlinked/) { get; set; } | True, wenn das Zahlenformat mit den Zellen verknüpft ist (so dass sich das Zahlenformat in den Beschriftungen ändert, wenn es sich in den Zellen ändert). |
| [Offset](../../aspose.cells.charts/ticklabels/offset/) { get; set; } | Liest und setzt den Abstand der Beschriftungen von der Kategorienachse. Dies gilt nur für die Kategorienachse (x). |
| [ReadingOrder](../../aspose.cells.charts/ticklabels/readingorder/) { get; set; } | Stellt die Lesereihenfolge des Textes dar. |
| [RotationAngle](../../aspose.cells.charts/ticklabels/rotationangle/) { get; set; } | Stellt den Textrotationswinkel im Uhrzeigersinn dar. |
| [TextDirection](../../aspose.cells.charts/ticklabels/textdirection/) { get; set; } | (**Obsolete.**) Stellt die Lesereihenfolge des Textes dar. |
| [TickLabelItems](../../aspose.cells.charts/ticklabels/ticklabelitems/) { get; } | Liest die angezeigten Tick‑Beschriftungen der Achse. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelsDemo
    {
        public static void TickLabelsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Füge NSeries (Diagrammdatenquelle) zum Diagramm hinzu, das vom Feld "A1" bis "B3" reicht.
            chart.NSeries.Add("A1:B3", true);

            // Zugriff auf die Werteachse
            Axis valueAxis = chart.ValueAxis;

            // Greifen Sie auf die Tick‑Beschriftungen der Werteachse zu
            TickLabels tickLabels = valueAxis.TickLabels;

            // Setzen Sie Eigenschaften der Tick‑Beschriftungen
            tickLabels.AutoScaleFont = true;
            tickLabels.BackgroundMode = BackgroundMode.Transparent;
            tickLabels.RotationAngle = 45;
            tickLabels.IsAutomaticRotation = false;
            tickLabels.NumberFormat = "0.00";
            tickLabels.Number = 2;
            tickLabels.NumberFormatLinked = true;
            tickLabels.Offset = 100;
            tickLabels.TextDirection = TextDirectionType.LeftToRight;
            tickLabels.ReadingOrder = TextDirectionType.LeftToRight;
            tickLabels.DirectionType = ChartTextDirectionType.Horizontal;
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // Speichere die Arbeitsmappe
            workbook.Save("TickLabelsExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


