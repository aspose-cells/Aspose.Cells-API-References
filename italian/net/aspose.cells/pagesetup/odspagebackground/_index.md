---
title: "PageSetup.ODSPageBackground"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Ottiene lo sfondo di ODS"
type: docs
url: /it/net/aspose.cells/pagesetup/odspagebackground/
---
## PageSetup.ODSPageBackground property

Ottiene lo sfondo di ODS.

```csharp
public OdsPageBackground ODSPageBackground { get; }
```

### Esempi

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
            
            // Imposta lo sfondo a colore
            background.Type = OdsPageBackgroundType.Color;
            background.Color = Color.LightGreen;
            
            // In alternativa, imposta lo sfondo grafico
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicType = OdsPageBackgroundGraphicType.Tile;
            background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.TopLeft;
            
            workbook.Save("ODSPageBackgroundDemo.ods");
        }
    }
}
```

### Vedi anche

* class [OdsPageBackground](../../../aspose.cells.ods/odspagebackground/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


