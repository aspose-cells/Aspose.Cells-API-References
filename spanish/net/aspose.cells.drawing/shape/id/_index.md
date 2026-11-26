---
title: "Shape.Id"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene el identificador de esta forma"
type: docs
url: /es/net/aspose.cells.drawing/shape/id/
---
## Shape.Id property

Obtiene el identificador de esta forma.

```csharp
public int Id { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIdDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Obtener y mostrar el ID de la forma
            int id = shape.Id;
            Console.WriteLine("Shape ID: " + id);

            // Modificar las propiedades de la forma
            shape.Name = "Rectangle1";
            shape.Text = "Shape with ID: " + id;

            // Guarda el libro de trabajo
            workbook.Save("ShapePropertyIdDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


