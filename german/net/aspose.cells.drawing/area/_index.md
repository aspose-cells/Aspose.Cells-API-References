---
title: "Klasse Area"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Area‑Klasse. Kapselt das Objekt, das ein Flächenformat repräsentiert"
type: docs
url: /de/net/aspose.cells.drawing/area/
---
## Area class

Kapselt das Objekt, das ein Flächenformat darstellt.

```csharp
public class Area
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Liest oder setzt die Hintergrundfarbe des `Area`. |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Stellt ein [`FillFormat`](./fillformat/)‑Objekt dar, das Füllformatierungs‑Eigenschaften für das angegebene Diagramm oder die angegebene Form enthält. |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Liest oder setzt die Vordergrundfarbe. |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Stellt die Formatierung des Bereichs dar. |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Wenn die Eigenschaft wahr ist und der Wert des Diagrammpunkts eine negative Zahl ist, werden die Vordergrundfarbe und die Hintergrundfarbe ausgetauscht. |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class AreaDemo
    {
        public static void AreaExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            // Hinzufügen eines neuen Arbeitsblatts zum Workbook-Objekt
            int sheetIndex = workbook.Worksheets.Add();
            // Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergabe seines Blattindexes
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Hinzufügen von Beispielwerten zu Zellen
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(-100);
            worksheet.Cells["A3"].PutValue(150);
            // Hinzufügen eines Diagramms zum Arbeitsblatt
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 15, 5);
            // Zugriff auf die Instanz des neu hinzugefügten Diagramms
            Chart chart = worksheet.Charts[chartIndex];
            // Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm von der Zelle "A1" bis "A3"
            chart.NSeries.Add("A1:A3", true);

            // Zugriff auf den Bereich der ersten NSeries
            Area area = chart.NSeries[0].Area;

            // Eigenschaften festlegen
            area.InvertIfNegative = true;
            area.ForegroundColor = Color.Red;
            area.BackgroundColor = Color.Yellow;
            area.Formatting = Aspose.Cells.Charts.FormattingType.Custom;
            area.Transparency = 0.5;

            // Die Excel-Datei speichern
            workbook.Save("AreaExample.xlsx");
            workbook.Save("AreaExample.pdf");

        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


