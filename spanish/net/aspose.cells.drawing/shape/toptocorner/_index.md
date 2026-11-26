---
title: "Shape.TopToCorner"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo en unidades de píxeles"
type: docs
url: /es/net/aspose.cells.drawing/shape/toptocorner/
---
## Shape.TopToCorner property

Obtiene y establece el desplazamiento vertical de la forma desde el borde superior de la hoja de cálculo, en unidades de píxeles.

```csharp
public int TopToCorner { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopToCornerDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una forma rectangular a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Establecer y mostrar la propiedad TopToCorner
            shape.TopToCorner = 50;
            Console.WriteLine("Shape TopToCorner: " + shape.TopToCorner);

            // Modificar la propiedad TopToCorner
            if (shape.TopToCorner == 50)
            {
                shape.TopToCorner = 20;
                Console.WriteLine("Updated Shape TopToCorner: " + shape.TopToCorner);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


