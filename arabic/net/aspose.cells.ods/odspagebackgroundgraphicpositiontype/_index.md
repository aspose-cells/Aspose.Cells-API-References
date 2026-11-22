---
title: "Enum OdsPageBackgroundGraphicPositionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Ods.OdsPageBackgroundGraphicPositionType enum. يمثل الموضع"
type: docs
url: /ar/net/aspose.cells.ods/odspagebackgroundgraphicpositiontype/
---
## OdsPageBackgroundGraphicPositionType enumeration

يمثل الموقع.

```csharp
public enum OdsPageBackgroundGraphicPositionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| TopLeft | `0` | أعلى اليسار. |
| TopCenter | `1` | أعلى الوسط. |
| TopRight | `2` | أعلى اليمين. |
| CenterLeft | `3` | وسط اليسار. |
| CenterCenter | `4` | وسط. |
| CenterRight | `5` | وسط اليمين. |
| BottomLeft | `6` | أسفل اليسار. |
| BottomCenter | `7` | أسفل الوسط. |
| BottomRight | `8` | أسفل اليمين. |

### أمثلة

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

### انظر أيضًا

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


