---
title: "Shape.IsEquation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Indica si la forma solo contiene una ecuación"
type: docs
url: /es/net/aspose.cells.drawing/shape/isequation/
---
## Shape.IsEquation property

Indica si la forma solo contiene una ecuación.

```csharp
public bool IsEquation { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsEquationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue una forma de ecuación con los parámetros correctos
            Shape equationShape = worksheet.Shapes.AddEquation(0, 0, 0, 0, 100, 100);
            equationShape.AlternativeText = "x^2 + y^2 = r^2";
            
            // Agregue una forma rectangular regular con los parámetros correctos
            Shape rectangleShape = worksheet.Shapes.AddRectangle(2, 0, 0, 0, 100, 100);

            foreach (Shape shape in worksheet.Shapes)
            {
                if (shape.IsEquation)
                {
                    Console.WriteLine("Shape is an equation: " + shape.AlternativeText);
                }
                else
                {
                    Console.WriteLine("Shape is not an equation");
                }
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


