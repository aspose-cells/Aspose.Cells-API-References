---
title: "Klass OdsPageBackground"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Ods.OdsPageBackground-klass. Representerar sidbakgrunden för ods"
type: docs
url: /sv/net/aspose.cells.ods/odspagebackground/
---
## OdsPageBackground class

Representerar sidbakgrunden för ods.

```csharp
public class OdsPageBackground
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [OdsPageBackground](odspagebackground/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Color](../../aspose.cells.ods/odspagebackground/color/) { get; set; } | Hämtar och anger bakgrundens färg. |
| [GraphicData](../../aspose.cells.ods/odspagebackground/graphicdata/) { get; set; } | Hämtar och anger grafikdata. |
| [GraphicPositionType](../../aspose.cells.ods/odspagebackground/graphicpositiontype/) { get; set; } | Hämtar och anger bakgrundsgrafikens position. |
| [GraphicType](../../aspose.cells.ods/odspagebackground/graphictype/) { get; set; } | Hämtar och anger sidbakgrundsgrafikens typ. |
| [IsLink](../../aspose.cells.ods/odspagebackground/islink/) { get; } | Indikerar om det är en länkad grafik. |
| [LinkedGraphic](../../aspose.cells.ods/odspagebackground/linkedgraphic/) { get; set; } | Hämtar och anger den länkade grafikens sökväg. |
| [Type](../../aspose.cells.ods/odspagebackground/type/) { get; set; } | Hämtar och anger sidbakgrundstypen. |

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Ods;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundDemo
    {
        public static void OdsPageBackgroundExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Kom åt PageSetup-objektet
            PageSetup pageSetup = sheet.PageSetup;

            // Åtkomst till ODSPageBackground-objektet
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Ställ in bakgrundstypen till Färg
            odsPageBackground.Type = OdsPageBackgroundType.Color;

            // Ange bakgrundsfärgen
            odsPageBackground.Color = Color.LightBlue;

            // Ange bakgrundsgrafikens typ
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;

            // Ange bakgrundsgrafikens position
            odsPageBackground.GraphicPositionType = OdsPageBackgroundGraphicPositionType.CenterCenter;

            // Ange den länkade grafikens sökväg (om någon)
            odsPageBackground.LinkedGraphic = "path/to/graphic.png";

            // Spara arbetsboken
            workbook.Save("OdsPageBackgroundExample.ods");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


