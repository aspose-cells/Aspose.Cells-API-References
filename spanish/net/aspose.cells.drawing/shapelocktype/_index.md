---
title: "Enum ShapeLockType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.ShapeLockType enum. Representa el tipo de la propiedad a bloquear"
type: docs
url: /es/net/aspose.cells.drawing/shapelocktype/
---
## ShapeLockType enumeration

Representa el tipo de la propiedad a bloquear.

```csharp
public enum ShapeLockType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Group | `0` | Grupo |
| AdjustHandles | `1` | AdjustHandles |
| Text | `2` | Texto |
| Points | `3` | Points |
| Crop | `4` | Crop |
| Selection | `5` | Selection |
| Move | `6` | Move |
| AspectRatio | `7` | AspectRatio |
| Rotation | `8` | Rotation |
| Ungroup | `9` | Ungroup |
| Resize | `10` | Resize |
| ShapeType | `11` | ShapeType |
| Arrowhead | `12` | Arrowhead |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapeLockTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una imagen a la hoja de cálculo
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];

            // Demostrar la funcionalidad de ShapeLockType
            picture.SetLockedProperty(Aspose.Cells.Drawing.ShapeLockType.AspectRatio, false);
            bool isAspectRatioLocked = picture.GetLockedProperty(Aspose.Cells.Drawing.ShapeLockType.AspectRatio);

            Console.WriteLine("Aspect Ratio locked: " + isAspectRatioLocked);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


