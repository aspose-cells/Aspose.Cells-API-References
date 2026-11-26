---
title: "PageSetup.ODSPageBackground"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Obtiene el fondo de ODS"
type: docs
url: /es/net/aspose.cells/pagesetup/odspagebackground/
---
## PageSetup.ODSPageBackground property

Obtiene el fondo de ODS.

```csharp
public OdsPageBackground ODSPageBackground { get; }
```

### Ejemplos

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
            
            // Establecer fondo de color
            background.Type = OdsPageBackgroundType.Color;
            background.Color = Color.LightGreen;
            
            // Alternativamente, establecer fondo gráfico
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicType = OdsPageBackgroundGraphicType.Tile;
            background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.TopLeft;
            
            workbook.Save("ODSPageBackgroundDemo.ods");
        }
    }
}
```

### Ver también

* class [OdsPageBackground](../../../aspose.cells.ods/odspagebackground/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


