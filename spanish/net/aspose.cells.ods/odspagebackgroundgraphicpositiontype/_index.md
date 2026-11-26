---
title: "Enum OdsPageBackgroundGraphicPositionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Ods.OdsPageBackgroundGraphicPositionType enum. Representa la posición"
type: docs
url: /es/net/aspose.cells.ods/odspagebackgroundgraphicpositiontype/
---
## OdsPageBackgroundGraphicPositionType enumeration

Representa la posición.

```csharp
public enum OdsPageBackgroundGraphicPositionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| TopLeft | `0` | Superior izquierda. |
| TopCenter | `1` | Superior centro. |
| TopRight | `2` | Superior derecha. |
| CenterLeft | `3` | Centro izquierda. |
| CenterCenter | `4` | Centro. |
| CenterRight | `5` | Centro derecha. |
| BottomLeft | `6` | Inferior izquierda. |
| BottomCenter | `7` | Inferior centro. |
| BottomRight | `8` | Inferior derecha. |

### Ejemplos

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

### Ver también

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


