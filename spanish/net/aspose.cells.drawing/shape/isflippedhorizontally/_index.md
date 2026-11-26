---
title: "Shape.IsFlippedHorizontally"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece si la forma está volteada horizontalmente"
type: docs
url: /es/net/aspose.cells.drawing/shape/isflippedhorizontally/
---
## Shape.IsFlippedHorizontally property

Obtiene y establece si la forma está volteada horizontalmente.

```csharp
public bool IsFlippedHorizontally { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsFlippedHorizontallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de ejemplo con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Verificar y voltear horizontalmente si aún no está volteada
            if (shape.IsFlippedHorizontally == false)
            {
                shape.IsFlippedHorizontally = true;
                Console.WriteLine("Shape was flipped horizontally");
            }
            else
            {
                Console.WriteLine("Shape was already flipped horizontally");
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


