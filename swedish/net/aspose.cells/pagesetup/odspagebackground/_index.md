---
title: "PageSetup.ODSPageBackground"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup egenskap. Hämtar bakgrunden för ODS"
type: docs
url: /sv/net/aspose.cells/pagesetup/odspagebackground/
---
## PageSetup.ODSPageBackground property

Hämtar bakgrunden för ODS.

```csharp
public OdsPageBackground ODSPageBackground { get; }
```

### Exempel

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
            
            // Ställ in färgad bakgrund
            background.Type = OdsPageBackgroundType.Color;
            background.Color = Color.LightGreen;
            
            // Alternativt, ange grafisk bakgrund
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicType = OdsPageBackgroundGraphicType.Tile;
            background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.TopLeft;
            
            workbook.Save("ODSPageBackgroundDemo.ods");
        }
    }
}
```

### Se även

* class [OdsPageBackground](../../../aspose.cells.ods/odspagebackground/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


