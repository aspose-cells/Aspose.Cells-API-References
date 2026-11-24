---
title: "Enum OdsPageBackgroundGraphicPositionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Ods.OdsPageBackgroundGraphicPositionType Enum. Repräsentiert die Position"
type: docs
url: /de/net/aspose.cells.ods/odspagebackgroundgraphicpositiontype/
---
## OdsPageBackgroundGraphicPositionType enumeration

Stellt die Position dar.

```csharp
public enum OdsPageBackgroundGraphicPositionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| TopLeft | `0` | Oben links. |
| TopCenter | `1` | Oben Mitte. |
| TopRight | `2` | Oben rechts. |
| CenterLeft | `3` | Mitte links. |
| CenterCenter | `4` | Mitte. |
| CenterRight | `5` | Mitte rechts. |
| BottomLeft | `6` | Unten links. |
| BottomCenter | `7` | Unten Mitte. |
| BottomRight | `8` | Unten rechts. |

### Beispiele

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

### Siehe auch

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


