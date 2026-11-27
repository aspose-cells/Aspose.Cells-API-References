---
title: "Class TilePicOption"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.TilePicOption-klass. Representerar kakelbild som textur"
type: docs
url: /sv/net/aspose.cells.drawing/tilepicoption/
---
## TilePicOption class

Representerar kakelbild som textur.

```csharp
public class TilePicOption
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [TilePicOption](tilepicoption/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing/tilepicoption/alignmenttype/) { get; set; } | Hämtar eller anger justeringen för kakling. |
| [MirrorType](../../aspose.cells.drawing/tilepicoption/mirrortype/) { get; set; } | Hämtar eller anger spegeltypen för kakling. |
| [OffsetX](../../aspose.cells.drawing/tilepicoption/offsetx/) { get; set; } | Hämtar eller anger X‑förskjutningen för kakelbilden. |
| [OffsetY](../../aspose.cells.drawing/tilepicoption/offsety/) { get; set; } | Hämtar eller anger Y‑förskjutningen för kakelbilden. |
| [ScaleX](../../aspose.cells.drawing/tilepicoption/scalex/) { get; set; } | Hämtar eller anger X‑skalan för kakelbilden. |
| [ScaleY](../../aspose.cells.drawing/tilepicoption/scaley/) { get; set; } | Hämtar eller anger Y‑skalan för kakelbilden. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett diagram för demonstration
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Ställ in fyllningstyp till textur
            chart.ChartArea.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Texture;

            // Läs in exempelbild (ersätt med faktisk sökväg)
            byte[] imageData = File.ReadAllBytes("sample.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // Skapa och konfigurera TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            tileOptions.ScaleX = 50;
            tileOptions.ScaleY = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = tileOptions;

            // Spara arbetsboken
            workbook.Save("TilePicOptionDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


