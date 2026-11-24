---
title: "Klasse Floor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.Floor‑Klasse. Kapselt das Objekt, das den Boden eines 3D‑Diagramms darstellt."
type: docs
url: /de/net/aspose.cells.charts/floor/
---
## Floor class

Kapselt das Objekt, das den Boden eines 3‑D-Diagramms darstellt.

```csharp
public class Floor : Area
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Liest oder setzt die Hintergrundfarbe des [`Area`](../../aspose.cells.drawing/area/). (Vererbt von [`Area`](../../aspose.cells.drawing/area/).) |
| [Border](../../aspose.cells.charts/floor/border/) { get; set; } | Liest oder setzt den Rand [`Line`](../../aspose.cells.drawing/line/). |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Stellt ein [`FillFormat`](../../aspose.cells.drawing/area/fillformat/) Objekt dar, das Füllformatierungs‑Eigenschaften für das angegebene Diagramm oder die Form enthält.(Vererbt von [`Area`](../../aspose.cells.drawing/area/).) |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Liest oder setzt die Vordergrundfarbe.(Vererbt von [`Area`](../../aspose.cells.drawing/area/).) |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Stellt die Formatierung des Bereichs dar.(Vererbt von [`Area`](../../aspose.cells.drawing/area/).) |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Wenn die Eigenschaft true ist und der Wert des Diagrammpunkts eine negative Zahl ist, werden die Vordergrund‑ und Hintergrundfarbe vertauscht.(Vererbt von [`Area`](../../aspose.cells.drawing/area/).) |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Liefert oder setzt den Transparenzgrad des Bereichs als Wert von 0.0 (undurchsichtig) bis 1.0 (klar).(Vererbt von [`Area`](../../aspose.cells.drawing/area/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FloorDemo
    {
        public static void FloorExample()
        {
            // Instanziieren Sie das Arbeitsmappen-Objekt
            Workbook workbook = new Workbook();

            // Zellsammlung abrufen
            Cells cells = workbook.Worksheets[0].Cells;

            // Werte in Zellen einfügen
            cells["A1"].PutValue(1);
            cells["A2"].PutValue(2);
            cells["A3"].PutValue(3);

            // Diagrammsammlung abrufen
            ChartCollection charts = workbook.Worksheets[0].Charts;

            // Ein neues Diagramm hinzufügen
            int index = charts.Add(ChartType.Column3DStacked, 5, 0, 15, 5);

            // Das neu hinzugefügte Diagramm abrufen
            Chart chart = charts[index];

            // nSeries des Diagramms festlegen
            chart.NSeries.Add("A1:A3", true);

            // Datenbeschriftungen anzeigen
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Boden des Diagramms abrufen
            Floor floor = chart.Floor;

            // Rand des Bodens rot setzen
            floor.Border.Color = Color.Red;

            // Füllformat festlegen
            floor.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.DiagonalDown, 2);

            // Zusätzliche Eigenschaften festlegen
            floor.BackgroundColor = Color.LightBlue;
            floor.ForegroundColor = Color.DarkBlue;
            floor.Formatting = FormattingType.Custom;
            floor.InvertIfNegative = true;
            floor.Transparency = 0.5;

            // Datei speichern
            workbook.Save(@"FloorExample.xlsx");
            workbook.Save(@"FloorExample.pdf");
        }
    }
}
```

### Siehe auch

* class [Area](../../aspose.cells.drawing/area/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


