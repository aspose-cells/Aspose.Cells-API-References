---
title: "Shape.TextHorizontalAlignment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Shape. Obtiene y establece el tipo de alineación horizontal del texto del shape"
type: docs
url: /es/net/aspose.cells.drawing/shape/texthorizontalalignment/
---
## Shape.TextHorizontalAlignment property

Obtiene y establece el tipo de alineación horizontal del texto de la forma.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Establecer texto y alineación
            shape.Text = "Sample Text";
            shape.TextHorizontalAlignment = TextAlignmentType.Center;

            // Cambiar la alineación si actualmente es Inferior
            if (shape.TextHorizontalAlignment == TextAlignmentType.Bottom)
            {
                shape.TextHorizontalAlignment = TextAlignmentType.Center;
            }

            // Guarda el libro de trabajo
            workbook.Save("ShapeTextAlignmentDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


