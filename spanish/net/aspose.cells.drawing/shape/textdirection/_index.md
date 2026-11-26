---
title: "Shape.TextDirection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene/Establece la dirección del flujo de texto para este objeto"
type: docs
url: /es/net/aspose.cells.drawing/shape/textdirection/
---
## Shape.TextDirection property

Obtiene/Establece la dirección del flujo de texto para este objeto.

```csharp
public TextDirectionType TextDirection { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextDirectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de cuadro de texto
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 100, 100);
            shape.Text = "Sample Text";

            // Establecer y demostrar la propiedad TextDirection
            shape.TextDirection = TextDirectionType.Context;
            Console.WriteLine("Initial TextDirection: " + shape.TextDirection);

            // Cambiar la dirección del texto
            shape.TextDirection = TextDirectionType.LeftToRight;
            Console.WriteLine("Updated TextDirection: " + shape.TextDirection);

            // Guarda el libro de trabajo
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


