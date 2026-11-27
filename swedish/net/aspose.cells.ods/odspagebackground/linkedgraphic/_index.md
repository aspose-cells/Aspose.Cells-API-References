---
title: "OdsPageBackground.LinkedGraphic"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsPageBackground egenskap. Hämtar och anger sökvägen till den länkade grafiken"
type: docs
url: /sv/net/aspose.cells.ods/odspagebackground/linkedgraphic/
---
## OdsPageBackground.LinkedGraphic property

Hämtar och anger den länkade grafikens sökväg.

```csharp
public string LinkedGraphic { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyLinkedGraphicDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            PageSetup pageSetup = worksheet.PageSetup;
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            odsPageBackground.Color = Color.LightBlue;
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;
            odsPageBackground.LinkedGraphic = "background_image.png";

            workbook.Save("OdsPageBackgroundLinkedGraphicDemo.ods");
        }
    }
}
```

### Se även

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


