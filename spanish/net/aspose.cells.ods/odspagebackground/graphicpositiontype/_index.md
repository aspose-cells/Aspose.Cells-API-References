---
title: "OdsPageBackground.GraphicPositionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OdsPageBackground. Obtiene y establece la posición del gráfico de fondo"
type: docs
url: /es/net/aspose.cells.ods/odspagebackground/graphicpositiontype/
---
## OdsPageBackground.GraphicPositionType property

Obtiene y establece la posición del gráfico de fondo.

```csharp
public OdsPageBackgroundGraphicPositionType GraphicPositionType { get; set; }
```

### Ejemplos

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

### Ver también

* enum [OdsPageBackgroundGraphicPositionType](../../odspagebackgroundgraphicpositiontype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


