---
title: "Enum OdsPageBackgroundType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Ods.OdsPageBackgroundType enum. Representerar sidbakgrundstypen för ods"
type: docs
url: /sv/net/aspose.cells.ods/odspagebackgroundtype/
---
## OdsPageBackgroundType enumeration

Representerar sidbakgrundstypen för ods.

```csharp
public enum OdsPageBackgroundType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen bakgrund. |
| Color | `1` | Formaterar bakgrunden med färg. |
| Graphic | `2` | Formaterar bakgrunden med bild. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;
    using System.Drawing;

    public class OdsPageBackgroundTypeDemo
    {
        public static void OdsPageBackgroundTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till PageSetup för kalkylbladet
            PageSetup pageSetup = worksheet.PageSetup;

            // Åtkomst till ODSPageBackground-egenskapen
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Ställ in bakgrundstypen till Färg
            odsPageBackground.Type = OdsPageBackgroundType.Color;

            // Ange bakgrundsfärgen
            odsPageBackground.Color = Color.LightBlue;

            // Spara arbetsboken
            workbook.Save("OdsPageBackgroundTypeExample.ods");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


