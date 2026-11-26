---
title: "Shape.HeightInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa la altura de la forma en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells.drawing/shape/heightinch/
---
## Shape.HeightInch property

Representa la altura de la forma, en unidades de pulgadas.

```csharp
public double HeightInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // Establecer y obtener la altura en pulgadas
            shape.HeightInch = 3;
            Console.WriteLine("Shape height (inches): " + shape.HeightInch);

            // Modificar la altura si se cumple la condición
            if (shape.HeightInch == 3)
            {
                shape.HeightInch = 1;
                Console.WriteLine("Modified shape height (inches): " + shape.HeightInch);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


