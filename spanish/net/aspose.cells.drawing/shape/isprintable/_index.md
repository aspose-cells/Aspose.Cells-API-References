---
title: "Shape.IsPrintable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Indica si el objeto es imprimible. Si es False, esta forma no se imprimirá al imprimir"
type: docs
url: /es/net/aspose.cells.drawing/shape/isprintable/
---
## Shape.IsPrintable property

Indica si el objeto es imprimible. Si False, esta forma no se imprimirá al imprimir.

```csharp
public bool IsPrintable { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsPrintableDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Demostrar la propiedad IsPrintable
            Console.WriteLine("Shape is printable initially: " + shape.IsPrintable);

            // Alternar la propiedad IsPrintable
            shape.IsPrintable = !shape.IsPrintable;
            Console.WriteLine("Shape is printable after toggle: " + shape.IsPrintable);

            // Establecer IsPrintable a false explícitamente
            shape.IsPrintable = false;
            Console.WriteLine("Shape is printable after setting to false: " + shape.IsPrintable);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


