---
title: "Enum MirrorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.MirrorType enum. Representa el tipo de espejo del relleno de textura"
type: docs
url: /es/net/aspose.cells.drawing/mirrortype/
---
## MirrorType enumeration

Representa el tipo de espejo del relleno de textura

```csharp
public enum MirrorType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Ninguno |
| Horizonal | `1` | Horizontal |
| Vertical | `2` | Vertical |
| Both | `3` | Ambos |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassMirrorTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue una forma para demostrar MirrorType
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 200);

            // Establezca el relleno de textura con diferentes tipos de espejo
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Horizonal;
            shape = worksheet.Shapes.AddRectangle(2, 0, 1, 100, 100, 200);
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Vertical;
            shape = worksheet.Shapes.AddRectangle(3, 0, 1, 100, 100, 200);
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.Both;
            shape = worksheet.Shapes.AddRectangle(4, 0, 1, 100, 100, 200);
            shape.Fill.TextureFill.TilePicOption.MirrorType = MirrorType.None;

            // Guardar el resultado
            workbook.Save("MirrorTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


