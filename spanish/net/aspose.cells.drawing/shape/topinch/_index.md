---
title: "Shape.TopInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa el desplazamiento vertical de la forma desde su fila superior en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells.drawing/shape/topinch/
---
## Shape.TopInch property

Representa el desplazamiento vertical de la forma desde su fila superior, en unidades de pulgadas.

```csharp
public double TopInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopInchDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Establecer y demostrar la propiedad TopInch
            shape.TopInch = 3;
            Console.WriteLine("Shape Top position (inches): " + shape.TopInch);

            // Modificar TopInch si es igual a 3
            if (shape.TopInch == 3)
            {
                shape.TopInch = 1;
                Console.WriteLine("Modified Shape Top position (inches): " + shape.TopInch);
            }

            // Guarda el libro de trabajo
            workbook.Save("ShapeTopInchDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


