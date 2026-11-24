---
title: "PageSetup.ODSPageBackground"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Ruft den Hintergrund von ODS ab."
type: docs
url: /de/net/aspose.cells/pagesetup/odspagebackground/
---
## PageSetup.ODSPageBackground property

Liest den Hintergrund von ODS.

```csharp
public OdsPageBackground ODSPageBackground { get; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyODSPageBackgroundDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            OdsPageBackground background = sheet.PageSetup.ODSPageBackground;
            
            // Farbigen Hintergrund festlegen
            background.Type = OdsPageBackgroundType.Color;
            background.Color = Color.LightGreen;
            
            // Alternativ kann ein grafischer Hintergrund festgelegt werden
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicType = OdsPageBackgroundGraphicType.Tile;
            background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.TopLeft;
            
            workbook.Save("ODSPageBackgroundDemo.ods");
        }
    }
}
```

### Siehe auch

* class [OdsPageBackground](../../../aspose.cells.ods/odspagebackground/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


