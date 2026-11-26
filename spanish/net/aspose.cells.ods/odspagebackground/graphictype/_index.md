---
title: "OdsPageBackground.GraphicType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OdsPageBackground. Obtiene y establece el tipo de gráfico de fondo de página"
type: docs
url: /es/net/aspose.cells.ods/odspagebackground/graphictype/
---
## OdsPageBackground.GraphicType property

Obtiene y establece el tipo de gráfico del fondo de página.

```csharp
public OdsPageBackgroundGraphicType GraphicType { get; set; }
```

### Ejemplos

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

### Ver también

* enum [OdsPageBackgroundGraphicType](../../odspagebackgroundgraphictype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


