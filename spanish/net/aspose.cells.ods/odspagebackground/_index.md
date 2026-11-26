---
title: "Clase OdsPageBackground"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Ods.OdsPageBackground. Representa el fondo de página de ODS"
type: docs
url: /es/net/aspose.cells.ods/odspagebackground/
---
## OdsPageBackground class

Representa el fondo de página de ODS.

```csharp
public class OdsPageBackground
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [OdsPageBackground](odspagebackground/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Color](../../aspose.cells.ods/odspagebackground/color/) { get; set; } | Obtiene y establece el color del fondo. |
| [GraphicData](../../aspose.cells.ods/odspagebackground/graphicdata/) { get; set; } | Obtiene y establece los datos gráficos. |
| [GraphicPositionType](../../aspose.cells.ods/odspagebackground/graphicpositiontype/) { get; set; } | Obtiene y establece la posición del gráfico de fondo. |
| [GraphicType](../../aspose.cells.ods/odspagebackground/graphictype/) { get; set; } | Obtiene y establece el tipo de gráfico del fondo de página. |
| [IsLink](../../aspose.cells.ods/odspagebackground/islink/) { get; } | Indica si es un gráfico vinculado. |
| [LinkedGraphic](../../aspose.cells.ods/odspagebackground/linkedgraphic/) { get; set; } | Obtiene y establece la ruta del gráfico vinculado. |
| [Type](../../aspose.cells.ods/odspagebackground/type/) { get; set; } | Obtiene y establece el tipo de fondo de página. |

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Ods;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundDemo
    {
        public static void OdsPageBackgroundExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Acceder al objeto PageSetup
            PageSetup pageSetup = sheet.PageSetup;

            // Acceder al objeto ODSPageBackground
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Establece el tipo de fondo a Color
            odsPageBackground.Type = OdsPageBackgroundType.Color;

            // Establezca el color de fondo
            odsPageBackground.Color = Color.LightBlue;

            // Establecer el tipo de gráfico de fondo
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;

            // Establecer la posición del gráfico de fondo
            odsPageBackground.GraphicPositionType = OdsPageBackgroundGraphicPositionType.CenterCenter;

            // Establecer la ruta del gráfico vinculado (si la hay)
            odsPageBackground.LinkedGraphic = "path/to/graphic.png";

            // Guarda el libro de trabajo
            workbook.Save("OdsPageBackgroundExample.ods");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


