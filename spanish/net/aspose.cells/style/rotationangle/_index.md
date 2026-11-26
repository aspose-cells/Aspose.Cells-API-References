---
title: "Style.RotationAngle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Representa el ángulo de rotación del texto"
type: docs
url: /es/net/aspose.cells/style/rotationangle/
---
## Style.RotationAngle property

Representa el ángulo de rotación del texto.

```csharp
public int RotationAngle { get; set; }
```

### Observaciones

0: No rotado.

255: De arriba a abajo.

-90: Downward.

90: Hacia arriba.

Puede establecer 255 o un valor entre -90 y 90.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree un estilo con diferentes ángulos de rotación
            Style style1 = workbook.CreateStyle();
            style1.RotationAngle = -90;
            worksheet.Cells["B2"].PutValue("Text rotated -90°");
            worksheet.Cells["B2"].SetStyle(style1);

            Style style2 = workbook.CreateStyle();
            style2.RotationAngle = 90;
            worksheet.Cells["C3"].PutValue("Text rotated 90°");
            worksheet.Cells["C3"].SetStyle(style2);

            Style style3 = workbook.CreateStyle();
            style3.RotationAngle = 255;
            worksheet.Cells["D4"].PutValue("Text rotated 255°");
            worksheet.Cells["D4"].SetStyle(style3);

            // Guarda el libro de trabajo
            workbook.Save("output_rotation_angles.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


