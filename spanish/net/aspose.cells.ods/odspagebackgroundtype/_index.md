---
title: "Enum OdsPageBackgroundType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Ods.OdsPageBackgroundType enum. Representa el tipo de fondo de página de ods"
type: docs
url: /es/net/aspose.cells.ods/odspagebackgroundtype/
---
## OdsPageBackgroundType enumeration

Representa el tipo de fondo de página de ods.

```csharp
public enum OdsPageBackgroundType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Sin fondo. |
| Color | `1` | Formatea el fondo con color. |
| Graphic | `2` | Formatea el fondo con imagen. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;
    using System.Drawing;

    public class OdsPageBackgroundTypeDemo
    {
        public static void OdsPageBackgroundTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder al PageSetup de la hoja de cálculo
            PageSetup pageSetup = worksheet.PageSetup;

            // Accede a la propiedad ODSPageBackground
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // Establece el tipo de fondo a Color
            odsPageBackground.Type = OdsPageBackgroundType.Color;

            // Establezca el color de fondo
            odsPageBackground.Color = Color.LightBlue;

            // Guarda el libro de trabajo
            workbook.Save("OdsPageBackgroundTypeExample.ods");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


