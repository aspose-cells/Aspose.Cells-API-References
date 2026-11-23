---
title: "Enum OdsPageBackgroundGraphicPositionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Ods.OdsPageBackgroundGraphicPositionType. Représente la position"
type: docs
url: /fr/net/aspose.cells.ods/odspagebackgroundgraphicpositiontype/
---
## OdsPageBackgroundGraphicPositionType enumeration

Représente la position.

```csharp
public enum OdsPageBackgroundGraphicPositionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| TopLeft | `0` | En haut à gauche. |
| TopCenter | `1` | En haut au centre. |
| TopRight | `2` | En haut à droite. |
| CenterLeft | `3` | Au centre à gauche. |
| CenterCenter | `4` | Centre. |
| CenterRight | `5` | Au centre à droite. |
| BottomLeft | `6` | En bas à gauche. |
| BottomCenter | `7` | En bas au centre. |
| BottomRight | `8` | En bas à droite. |

### Exemples

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

### Voir aussi

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


