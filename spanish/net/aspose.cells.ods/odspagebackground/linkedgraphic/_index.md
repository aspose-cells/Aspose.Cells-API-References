---
title: "OdsPageBackground.LinkedGraphic"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OdsPageBackground. Obtiene y establece la ruta del gráfico vinculado"
type: docs
url: /es/net/aspose.cells.ods/odspagebackground/linkedgraphic/
---
## OdsPageBackground.LinkedGraphic property

Obtiene y establece la ruta del gráfico vinculado.

```csharp
public string LinkedGraphic { get; set; }
```

### Ejemplos

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

### Ver también

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


