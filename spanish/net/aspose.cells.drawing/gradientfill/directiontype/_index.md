---
title: "GradientFill.DirectionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GradientFill. Obtiene el tipo de dirección del degradado"
type: docs
url: /es/net/aspose.cells.drawing/gradientfill/directiontype/
---
## GradientFill.DirectionType property

Obtiene el tipo de dirección del degradado.

```csharp
public GradientDirectionType DirectionType { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyDirectionTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma para demostrar el relleno de degradado
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 5, 5);

            // Establecer propiedades del relleno de degradado
            FillFormat fillFormat = shape.Fill;
            fillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.LightBlue, GradientStyleType.DiagonalDown, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Salida del tipo de dirección del gradiente
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Guarda el libro de trabajo
            workbook.Save("GradientDirectionTypeExample.xlsx");
        }
    }
}
```

### Ver también

* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


