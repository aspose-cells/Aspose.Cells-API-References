---
title: "Shape.WidthPt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Representa el ancho de la forma en unidades de punto"
type: docs
url: /es/net/aspose.cells.drawing/shape/widthpt/
---
## Shape.WidthPt property

Representa el ancho de la forma, en unidades de punto.

```csharp
public double WidthPt { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthPtDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Establecer y obtener el ancho en puntos
            shape.WidthPt = 150;
            Console.WriteLine("Shape width in points: " + shape.WidthPt);

            // Modificar el ancho si se cumple la condición
            if (shape.WidthPt == 150)
            {
                shape.WidthPt = 100;
                Console.WriteLine("Modified shape width in points: " + shape.WidthPt);
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


