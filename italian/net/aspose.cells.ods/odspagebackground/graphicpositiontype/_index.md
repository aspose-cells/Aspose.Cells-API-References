---
title: "OdsPageBackground.GraphicPositionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OdsPageBackground. Ottiene e imposta la posizione grafica dello sfondo"
type: docs
url: /it/net/aspose.cells.ods/odspagebackground/graphicpositiontype/
---
## OdsPageBackground.GraphicPositionType property

Ottiene e imposta la posizione della grafica di sfondo.

```csharp
public OdsPageBackgroundGraphicPositionType GraphicPositionType { get; set; }
```

### Esempi

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

### Vedi anche

* enum [OdsPageBackgroundGraphicPositionType](../../odspagebackgroundgraphicpositiontype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


