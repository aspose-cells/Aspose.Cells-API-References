---
title: "Shape.IsTextWrapped"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece el tipo de ajuste de texto de la forma que contiene texto"
type: docs
url: /es/net/aspose.cells.drawing/shape/istextwrapped/
---
## Shape.IsTextWrapped property

Obtiene y establece el tipo de ajuste de texto de la forma que contiene texto.

```csharp
public bool IsTextWrapped { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma y establecer texto
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            shape.Text = "This is a sample text that will demonstrate text wrapping functionality";

            // Demostrar la propiedad IsTextWrapped
            Console.WriteLine("Initial IsTextWrapped value: " + shape.IsTextWrapped);
            
            // Alternar el ajuste de texto
            shape.IsTextWrapped = !shape.IsTextWrapped;
            Console.WriteLine("After toggle, IsTextWrapped value: " + shape.IsTextWrapped);

            // Guarda el libro de trabajo
            workbook.Save("ShapeTextWrappingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


