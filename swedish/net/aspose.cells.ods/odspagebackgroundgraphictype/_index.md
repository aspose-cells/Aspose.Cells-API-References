---
title: "Enum OdsPageBackgroundGraphicType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Ods.OdsPageBackgroundGraphicType enum. Representerar typen av formateringsbakgrund för sidan med bild"
type: docs
url: /sv/net/aspose.cells.ods/odspagebackgroundgraphictype/
---
## OdsPageBackgroundGraphicType enumeration

Representerar typen av formatering av sidbakgrund med bild.

```csharp
public enum OdsPageBackgroundGraphicType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Position | `0` | Ställ in bilden på en specifik position. |
| Area | `1` | Sträck bilden. |
| Tile | `2` | Upprepa och upprepa bilden. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;
    using System.Drawing;

    public class OdsPageBackgroundGraphicTypeDemo
    {
        public static void OdsPageBackgroundGraphicTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till PageSetup för kalkylbladet
            PageSetup pageSetup = worksheet.PageSetup;

            // Åtkomst till ODSPageBackground i PageSetup
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Ange bakgrundsfärgen
            odsPageBackground.Color = Color.LightBlue;

            // Ställ in bakgrundsgrafiktypen till Tile
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;

            // Ange den länkade grafikens sökväg (förutsatt att bilden finns i samma katalog som den körbara filen)
            odsPageBackground.LinkedGraphic = "background_image.png";

            // Spara arbetsboken
            workbook.Save("OdsPageBackgroundGraphicTypeExample.ods");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


