---
title: "Enum OdsPageBackgroundGraphicPositionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Ods.OdsPageBackgroundGraphicPositionType enum. Pozisyonu temsil eder"
type: docs
url: /tr/net/aspose.cells.ods/odspagebackgroundgraphicpositiontype/
---
## OdsPageBackgroundGraphicPositionType enumeration

Pozisyonu temsil eder.

```csharp
public enum OdsPageBackgroundGraphicPositionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| TopLeft | `0` | Sol üst. |
| TopCenter | `1` | Üst orta. |
| TopRight | `2` | Sağ üst. |
| CenterLeft | `3` | Sol orta. |
| CenterCenter | `4` | Orta. |
| CenterRight | `5` | Sağ orta. |
| BottomLeft | `6` | Sol alt. |
| BottomCenter | `7` | Alt orta. |
| BottomRight | `8` | Sağ alt. |

### Örnekler

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

### Ayrıca Bakınız

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


