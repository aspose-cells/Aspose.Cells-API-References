---
title: "OdsPageBackground.GraphicType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsPageBackground egenskap. Hämtar och anger sidans bakgrundsgrafiktyp"
type: docs
url: /sv/net/aspose.cells.ods/odspagebackground/graphictype/
---
## OdsPageBackground.GraphicType property

Hämtar och anger sidbakgrundsgrafikens typ.

```csharp
public OdsPageBackgroundGraphicType GraphicType { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyGraphicTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            PageSetup pageSetup = sheet.PageSetup;
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;
            
            odsPageBackground.Type = OdsPageBackgroundType.Graphic;
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;
            odsPageBackground.LinkedGraphic = "background.png";
            
            workbook.Save("OdsPageBackgroundGraphicTypeDemo.ods");
        }
    }
}
```

### Se även

* enum [OdsPageBackgroundGraphicType](../../odspagebackgroundgraphictype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


