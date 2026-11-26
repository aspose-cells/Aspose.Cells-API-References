---
title: "Shape.WidthInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa el ancho de la forma en unidades de pulgada"
type: docs
url: /es/net/aspose.cells.drawing/shape/widthinch/
---
## Shape.WidthInch property

Representa el ancho de la forma, en unidades de pulgada.

```csharp
public double WidthInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // Establecer el ancho en pulgadas
            shape.WidthInch = 3;
            Console.WriteLine("Shape width (inches): " + shape.WidthInch);

            // Modificar el ancho si se cumple la condición
            if (shape.WidthInch == 3)
            {
                shape.WidthInch = 1;
                Console.WriteLine("Modified shape width (inches): " + shape.WidthInch);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


