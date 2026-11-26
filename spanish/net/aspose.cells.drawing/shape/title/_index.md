---
title: "Shape.Title"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Shape. Especifica el título del objeto forma actual"
type: docs
url: /es/net/aspose.cells.drawing/shape/title/
---
## Shape.Title property

Especifica el título (leyenda) del objeto forma actual.

```csharp
public string Title { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTitleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Establecer el título de la forma
            shape.Title = "title1";

            // Verificar que el título se haya establecido
            Console.WriteLine("Shape title: " + shape.Title);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


