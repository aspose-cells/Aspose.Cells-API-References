---
title: "Enumeración BevelType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.BevelType. Representa una configuración predefinida para un tipo de bisel que se puede aplicar a una forma en 3D"
type: docs
url: /es/net/aspose.cells.drawing/beveltype/
---
## BevelType enumeration

Representa un preset para un tipo de bisel que puede aplicarse a una forma en 3D.

```csharp
public enum BevelType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Sin bisel |
| Angle | `1` | Ángulo |
| ArtDeco | `2` | Art déco |
| Circle | `3` | Círculo |
| Convex | `4` | Convexo |
| CoolSlant | `5` | Inclinación fresca |
| Cross | `6` | Cruz |
| Divot | `7` | Hueco |
| HardEdge | `8` | Borde duro |
| RelaxedInset | `9` | Inserción relajada |
| Riblet | `10` | Estría |
| Slope | `11` | Pendiente |
| SoftRound | `12` | Redondez suave |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class BevelTypeDemo
    {
        public static void BevelTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            var shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 0, 2, 0, 100, 100);

            // Acceder al formato 3D de la forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Establecer el tipo y dimensiones del bisel superior
            threeDFormat.TopBevelType = BevelType.SoftRound;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;

            // Establecer el tipo y dimensiones del bisel inferior
            threeDFormat.BottomBevelType = BevelType.Divot;
            threeDFormat.BottomBevelWidth = 5;
            threeDFormat.BottomBevelHeight = 5;

            // Guarda el libro de trabajo
            workbook.Save("BevelTypeExample.xlsx");
            workbook.Save("BevelTypeExample.pdf");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


