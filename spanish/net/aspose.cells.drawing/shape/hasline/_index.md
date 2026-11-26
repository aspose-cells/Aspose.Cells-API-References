---
title: "Shape.HasLine"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece si el borde de línea de la forma es visible"
type: docs
url: /es/net/aspose.cells.drawing/shape/hasline/
---
## Shape.HasLine property

Obtiene y establece la visibilidad del borde de línea de la forma.

```csharp
public bool HasLine { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHasLineDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de ejemplo con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            // Demostrar la propiedad HasLine
            Console.WriteLine("Shape initially has line: " + shape.HasLine);
            
            // Eliminar la línea
            shape.HasLine = false;
            Console.WriteLine("After setting HasLine to false: " + shape.HasLine);
            
            // Agregar la línea nuevamente
            shape.HasLine = true;
            Console.WriteLine("After setting HasLine to true: " + shape.HasLine);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


