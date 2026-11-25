---
title: "OdsPageBackground.LinkedGraphic"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OdsPageBackground. Ottiene e imposta il percorso della grafica collegata"
type: docs
url: /it/net/aspose.cells.ods/odspagebackground/linkedgraphic/
---
## OdsPageBackground.LinkedGraphic property

Ottiene e imposta il percorso della grafica collegata.

```csharp
public string LinkedGraphic { get; set; }
```

### Esempi

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

### Vedi anche

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


