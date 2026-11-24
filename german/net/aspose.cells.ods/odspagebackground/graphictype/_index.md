---
title: "OdsPageBackground.GraphicType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OdsPageBackground-Eigenschaft. Liest und schreibt den Grafiktyp des Seitenhintergrunds."
type: docs
url: /de/net/aspose.cells.ods/odspagebackground/graphictype/
---
## OdsPageBackground.GraphicType property

Liest und setzt den Typ der Seitenhintergrundgrafik.

```csharp
public OdsPageBackgroundGraphicType GraphicType { get; set; }
```

### Beispiele

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

### Siehe auch

* enum [OdsPageBackgroundGraphicType](../../odspagebackgroundgraphictype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


