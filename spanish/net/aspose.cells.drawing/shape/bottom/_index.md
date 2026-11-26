---
title: "Shape.Bottom"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa el ancho del desplazamiento vertical de la forma desde su fila de esquina inferior en unidades de píxeles"
type: docs
url: /es/net/aspose.cells.drawing/shape/bottom/
---
## Shape.Bottom property

Representa el ancho del desplazamiento vertical de la forma desde la fila de su esquina inferior, en unidades de píxeles.

```csharp
public int Bottom { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyBottomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de ejemplo con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Establecer posición inicial
            shape.Top = 200;
            shape.Left = 200;

            // Demostrar la propiedad Bottom
            Console.WriteLine("Original Bottom position: " + shape.Bottom);

            // Modificar la posición Bottom
            if (shape.Bottom == 300)  // 200 (Top) + 100 (Height)
            {
                shape.Bottom = 250;  // This will change the Top position (250 - 100 = 150)
                Console.WriteLine("New Bottom position: " + shape.Bottom);
                Console.WriteLine("New Top position: " + shape.Top);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


