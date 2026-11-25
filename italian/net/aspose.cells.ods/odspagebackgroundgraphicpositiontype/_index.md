---
title: "Enum OdsPageBackgroundGraphicPositionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Ods.OdsPageBackgroundGraphicPositionType enum. Rappresenta la posizione"
type: docs
url: /it/net/aspose.cells.ods/odspagebackgroundgraphicpositiontype/
---
## OdsPageBackgroundGraphicPositionType enumeration

Rappresenta la posizione.

```csharp
public enum OdsPageBackgroundGraphicPositionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| TopLeft | `0` | In alto a sinistra. |
| TopCenter | `1` | In alto al centro. |
| TopRight | `2` | In alto a destra. |
| CenterLeft | `3` | Al centro a sinistra. |
| CenterCenter | `4` | Al centro. |
| CenterRight | `5` | Al centro a destra. |
| BottomLeft | `6` | In basso a sinistra. |
| BottomCenter | `7` | In basso al centro. |
| BottomRight | `8` | In basso a destra. |

### Esempi

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

### Vedi anche

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


