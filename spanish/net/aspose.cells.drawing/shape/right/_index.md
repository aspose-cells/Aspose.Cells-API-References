---
title: "Shape.Right"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa el ancho del desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha, en unidades de píxeles"
type: docs
url: /es/net/aspose.cells.drawing/shape/right/
---
## Shape.Right property

Representa el ancho del desplazamiento horizontal de la forma desde la columna de su esquina inferior derecha, en unidades de píxeles.

```csharp
public int Right { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRightDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Establezca y obtenga la propiedad Right
            shape.Right = 200;
            Console.WriteLine("Shape Right position: " + shape.Right);

            // Modifique la propiedad Right condicionalmente
            if (shape.Right == 200)
                shape.Right = 150;

            Console.WriteLine("Modified Shape Right position: " + shape.Right);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


