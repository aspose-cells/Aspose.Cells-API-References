---
title: "OdsPageBackground.GraphicPositionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsPageBackground-egenskap. Hämtar och anger bakgrundsgrafikens position"
type: docs
url: /sv/net/aspose.cells.ods/odspagebackground/graphicpositiontype/
---
## OdsPageBackground.GraphicPositionType property

Hämtar och anger bakgrundsgrafikens position.

```csharp
public OdsPageBackgroundGraphicPositionType GraphicPositionType { get; set; }
```

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyGraphicPositionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            PageSetup pageSetup = sheet.PageSetup;
            OdsPageBackground background = pageSetup.ODSPageBackground;

            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicType = OdsPageBackgroundGraphicType.Tile;
            background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.CenterCenter;
            background.LinkedGraphic = "sample/image.png";

            workbook.Save("OdsPageBackgroundGraphicPositionDemo.ods");
        }
    }
}
```

### Se även

* enum [OdsPageBackgroundGraphicPositionType](../../odspagebackgroundgraphicpositiontype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


