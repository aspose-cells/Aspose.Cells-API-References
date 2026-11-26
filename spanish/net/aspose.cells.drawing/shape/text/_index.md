---
title: "Shape.Text"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece el texto de esta forma"
type: docs
url: /es/net/aspose.cells.drawing/shape/text/
---
## Shape.Text property

Obtiene y establece el texto de esta forma.

```csharp
public string Text { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un shape rectangular con los parámetros correctos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Establezca el texto si es nulo
            if (shape.Text == null)
            {
                shape.Text = "This is a test.";
            }

            // Modifique el texto
            shape.Text = "Updated text demo";

            // Guarda el libro de trabajo
            workbook.Save("ShapeTextDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


