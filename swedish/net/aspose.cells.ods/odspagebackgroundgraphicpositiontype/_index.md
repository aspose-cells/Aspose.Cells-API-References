---
title: "Enum OdsPageBackgroundGraphicPositionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Ods.OdsPageBackgroundGraphicPositionType enum. Representerar positionen"
type: docs
url: /sv/net/aspose.cells.ods/odspagebackgroundgraphicpositiontype/
---
## OdsPageBackgroundGraphicPositionType enumeration

Representerar positionen.

```csharp
public enum OdsPageBackgroundGraphicPositionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| TopLeft | `0` | Överst till vänster. |
| TopCenter | `1` | Överst i mitten. |
| TopRight | `2` | Överst till höger. |
| CenterLeft | `3` | Centrerat till vänster. |
| CenterCenter | `4` | Centrerat. |
| CenterRight | `5` | Centrerat till höger. |
| BottomLeft | `6` | Nederst till vänster. |
| BottomCenter | `7` | Nederst i mitten. |
| BottomRight | `8` | Nederst till höger. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class OdsClassOdsPageBackgroundGraphicPositionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            PageSetup pageSetup = sheet.PageSetup;
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;
            
            odsPageBackground.Type = OdsPageBackgroundType.Color;
            odsPageBackground.Color = Color.LightBlue;
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;
            odsPageBackground.GraphicPositionType = OdsPageBackgroundGraphicPositionType.CenterCenter;
            
            workbook.Save("OdsPageBackgroundExample.ods");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


