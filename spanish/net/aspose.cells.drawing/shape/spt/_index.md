---
title: "Shape.Spt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Especifica un número opcional que una aplicación puede usar para asociar la forma particular con un tipo de forma definido"
type: docs
url: /es/net/aspose.cells.drawing/shape/spt/
---
## Shape.Spt property

Especifica un número opcional que una aplicación puede usar para asociar la forma particular con un tipo de forma definido.

```csharp
public int Spt { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySptDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un shape rectangular con los parámetros correctos
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 100, 100, 100, 100);

            // Obtener y mostrar la propiedad Spt
            int spt = shape.Spt;
            Console.WriteLine("Shape Spt value: " + spt);

            // Crear una nueva forma ovalada para demostrar un valor Spt diferente
            Shape ovalShape = worksheet.Shapes.AddShape(MsoDrawingType.Oval, 1, 1, 100, 100, 100, 100);
            Console.WriteLine("Oval shape Spt value: " + ovalShape.Spt);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


