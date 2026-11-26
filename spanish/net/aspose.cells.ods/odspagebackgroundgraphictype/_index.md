---
title: "Enumeración OdsPageBackgroundGraphicType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Ods.OdsPageBackgroundGraphicType enum. Representa el tipo de fondo de página de formato con imagen"
type: docs
url: /es/net/aspose.cells.ods/odspagebackgroundgraphictype/
---
## OdsPageBackgroundGraphicType enumeration

Representa el tipo de formato de fondo de página con imagen.

```csharp
public enum OdsPageBackgroundGraphicType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Position | `0` | Establezca la imagen en una posición específica. |
| Area | `1` | Estire la imagen. |
| Tile | `2` | Repita y repita la imagen. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;
    using System.Drawing;

    public class OdsPageBackgroundGraphicTypeDemo
    {
        public static void OdsPageBackgroundGraphicTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder al PageSetup de la hoja de cálculo
            PageSetup pageSetup = worksheet.PageSetup;

            // Acceda al ODSPageBackground del PageSetup
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Establezca el color de fondo
            odsPageBackground.Color = Color.LightBlue;

            // Establezca el tipo de gráfico de fondo a Tile
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;

            // Establezca la ruta del gráfico vinculado (suponiendo que la imagen esté en el mismo directorio que el ejecutable)
            odsPageBackground.LinkedGraphic = "background_image.png";

            // Guarda el libro de trabajo
            workbook.Save("OdsPageBackgroundGraphicTypeExample.ods");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


