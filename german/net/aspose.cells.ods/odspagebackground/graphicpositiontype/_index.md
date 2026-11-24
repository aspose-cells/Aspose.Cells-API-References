---
title: "OdsPageBackground.GraphicPositionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OdsPageBackground-Eigenschaft. Gibt die Position der Hintergrundgrafik zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.ods/odspagebackground/graphicpositiontype/
---
## OdsPageBackground.GraphicPositionType property

Liest und setzt die Position der Hintergrundgrafik.

```csharp
public OdsPageBackgroundGraphicPositionType GraphicPositionType { get; set; }
```

### Beispiele

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

### Siehe auch

* enum [OdsPageBackgroundGraphicPositionType](../../odspagebackgroundgraphicpositiontype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


