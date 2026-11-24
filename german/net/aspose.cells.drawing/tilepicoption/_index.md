---
title: "Klasse TilePicOption"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.TilePicOption Klasse. Stellt ein Kachelbild als Textur dar"
type: docs
url: /de/net/aspose.cells.drawing/tilepicoption/
---
## TilePicOption class

Stellt ein Kachelbild als Textur dar.

```csharp
public class TilePicOption
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [TilePicOption](tilepicoption/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing/tilepicoption/alignmenttype/) { get; set; } | Liest oder setzt die Ausrichtung für das Kacheln. |
| [MirrorType](../../aspose.cells.drawing/tilepicoption/mirrortype/) { get; set; } | Liest oder setzt den Spiegeltyp für das Kacheln. |
| [OffsetX](../../aspose.cells.drawing/tilepicoption/offsetx/) { get; set; } | Liest oder setzt den X‑Versatz für das Kachelbild. |
| [OffsetY](../../aspose.cells.drawing/tilepicoption/offsety/) { get; set; } | Liest oder setzt den Y‑Versatz für das Kachelbild. |
| [ScaleX](../../aspose.cells.drawing/tilepicoption/scalex/) { get; set; } | Liest oder setzt die X‑Skalierung für das Kachelbild. |
| [ScaleY](../../aspose.cells.drawing/tilepicoption/scaley/) { get; set; } | Liest oder setzt die Y‑Skalierung für das Kachelbild. |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTilePicOptionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Diagramm zur Demonstration hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Setze den Fülltyp auf Textur
            chart.ChartArea.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Texture;

            // Lade Beispielbild (mit tatsächlichem Pfad ersetzen)
            byte[] imageData = File.ReadAllBytes("sample.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // Erstellen und konfigurieren Sie TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            tileOptions.ScaleX = 50;
            tileOptions.ScaleY = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = tileOptions;

            // Speichere die Arbeitsmappe
            workbook.Save("TilePicOptionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


