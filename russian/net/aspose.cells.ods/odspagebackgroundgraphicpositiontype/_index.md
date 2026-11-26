---
title: "Перечисление OdsPageBackgroundGraphicPositionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Ods.OdsPageBackgroundGraphicPositionType. Представляет позицию"
type: docs
url: /ru/net/aspose.cells.ods/odspagebackgroundgraphicpositiontype/
---
## OdsPageBackgroundGraphicPositionType enumeration

Представляет позицию.

```csharp
public enum OdsPageBackgroundGraphicPositionType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| TopLeft | `0` | Сверху слева. |
| TopCenter | `1` | Сверху по центру. |
| TopRight | `2` | Сверху справа. |
| CenterLeft | `3` | По центру слева. |
| CenterCenter | `4` | По центру. |
| CenterRight | `5` | По центру справа. |
| BottomLeft | `6` | Снизу слева. |
| BottomCenter | `7` | Снизу по центру. |
| BottomRight | `8` | Снизу справа. |

### Примеры

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

### См. также

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


