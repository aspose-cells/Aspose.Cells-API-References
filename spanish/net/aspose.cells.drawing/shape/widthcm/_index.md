---
title: "Shape.WidthCM"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa el ancho de la forma en unidades de centímetros"
type: docs
url: /es/net/aspose.cells.drawing/shape/widthcm/
---
## Shape.WidthCM property

Representa el ancho de la forma, en unidades de centímetros.

```csharp
public double WidthCM { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 100, 100);

            // Establecer el ancho en centímetros
            shape.WidthCM = 3.5;
            Console.WriteLine("Shape width set to: " + shape.WidthCM + " cm");

            // Modificar el ancho si coincide con una condición
            if (shape.WidthCM == 3.5)
            {
                shape.WidthCM = 2.0;
                Console.WriteLine("Shape width changed to: " + shape.WidthCM + " cm");
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


