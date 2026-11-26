---
title: "Enum RectangleAlignmentType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.RectangleAlignmentType enum. Representa cómo posicionar dos rectángulos entre sí"
type: docs
url: /es/net/aspose.cells.drawing/rectanglealignmenttype/
---
## RectangleAlignmentType enumeration

Representa cómo posicionar dos rectángulos entre sí.

```csharp
public enum RectangleAlignmentType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Bottom | `0` | Inferior |
| BottomLeft | `1` | BottomLeft |
| BottomRight | `2` | BottomRight |
| Center | `3` | Center |
| Left | `4` | Left |
| Right | `5` | Right |
| Top | `6` | Top |
| TopLeft | `7` | TopLeft |
| TopRight | `8` | TopRight |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassRectangleAlignmentTypeDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar una forma de rectángulo para demostrar la alineación
                Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 0, 200, 100, 100);

                // Demostrar diferentes tipos de alineación
                Console.WriteLine("Available RectangleAlignmentType values:");
                Console.WriteLine("Bottom: " + RectangleAlignmentType.Bottom);
                Console.WriteLine("BottomLeft: " + RectangleAlignmentType.BottomLeft);
                Console.WriteLine("BottomRight: " + RectangleAlignmentType.BottomRight);
                Console.WriteLine("Center: " + RectangleAlignmentType.Center);
                Console.WriteLine("Left: " + RectangleAlignmentType.Left);
                Console.WriteLine("Right: " + RectangleAlignmentType.Right);
                Console.WriteLine("Top: " + RectangleAlignmentType.Top);
                Console.WriteLine("TopLeft: " + RectangleAlignmentType.TopLeft);
                Console.WriteLine("TopRight: " + RectangleAlignmentType.TopRight);

                // Establecer la alineación basada en uno de los valores del enum
                rectangle.TextHorizontalAlignment = TextAlignmentType.Center;
                rectangle.TextVerticalAlignment = TextAlignmentType.Center;

                // Guarda el libro de trabajo
                workbook.Save("RectangleAlignmentTypeDemo.xlsx");
                Console.WriteLine("RectangleAlignmentType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating RectangleAlignmentType: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


