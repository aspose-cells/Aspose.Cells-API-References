---
title: "Shape.LeftToCorner"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.drawing/shape/lefttocorner/
---
## Shape.LeftToCorner property

Obtiene y establece el desplazamiento horizontal de la forma desde el borde izquierdo de la hoja de cálculo.

```csharp
public int LeftToCorner { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftToCornerDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un shape rectangular con los parámetros correctos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Establezca y demuestre la propiedad LeftToCorner
            shape.LeftToCorner = 50;
            Console.WriteLine("Shape LeftToCorner value: " + shape.LeftToCorner);

            // Modifique LeftToCorner si es igual a un valor específico
            if (shape.LeftToCorner == 50)
            {
                shape.LeftToCorner = 30;
                Console.WriteLine("Modified LeftToCorner value: " + shape.LeftToCorner);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


