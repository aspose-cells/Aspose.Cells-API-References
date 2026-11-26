---
title: "Enum GradientFillType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.GradientFillType enum. Representa todos los tipos de relleno de degradado"
type: docs
url: /es/net/aspose.cells.drawing/gradientfilltype/
---
## GradientFillType enumeration

Representa todos los tipos de relleno de degradado.

```csharp
public enum GradientFillType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Linear | `0` | Lineal |
| Radial | `1` | Radial |
| Rectangle | `2` | Rectángulo |
| Path | `3` | Ruta |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassGradientFillTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma para demostrar el relleno de degradado
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 5, 20);

            // Obtener el formato de relleno
            FillFormat fillFormat = shape.Fill;

            // Establecer el tipo de relleno de degradado y sus propiedades
            fillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.LightBlue, GradientStyleType.Horizontal, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Salida del tipo de dirección del degradado
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Guarda el libro de trabajo
            workbook.Save("GradientFillTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


