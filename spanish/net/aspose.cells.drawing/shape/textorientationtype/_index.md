---
title: "Shape.TextOrientationType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece el tipo de orientación del texto de la forma"
type: docs
url: /es/net/aspose.cells.drawing/shape/textorientationtype/
---
## Shape.TextOrientationType property

Obtiene y establece el tipo de orientación del texto de la forma.

```csharp
public TextOrientationType TextOrientationType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextOrientationTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);

            // Establecer texto para la forma
            shape.Text = "Sample Text";

            // Verificar y modificar la orientación del texto
            if (shape.TextOrientationType == TextOrientationType.NoRotation)
            {
                shape.TextOrientationType = TextOrientationType.TopToBottom;
            }

            // Guarda el libro de trabajo
            workbook.Save("ShapeTextOrientationDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextOrientationType](../../../aspose.cells/textorientationtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


