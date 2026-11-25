---
title: "OdsPageBackground.GraphicType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OdsPageBackground. Ottiene e imposta il tipo di grafica di sfondo della pagina"
type: docs
url: /it/net/aspose.cells.ods/odspagebackground/graphictype/
---
## OdsPageBackground.GraphicType property

Ottiene e imposta il tipo di grafica di sfondo della pagina.

```csharp
public OdsPageBackgroundGraphicType GraphicType { get; set; }
```

### Esempi

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

### Vedi anche

* enum [OdsPageBackgroundGraphicType](../../odspagebackgroundgraphictype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


