---
title: "Shape.TextVerticalAlignment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Shape. Obtiene y establece el tipo de alineación vertical del texto de la forma"
type: docs
url: /es/net/aspose.cells.drawing/shape/textverticalalignment/
---
## Shape.TextVerticalAlignment property

Obtiene y establece el tipo de alineación vertical del texto de la forma.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Establecer texto y alineación
            shape.Text = "Vertical Alignment Demo";
            shape.TextVerticalAlignment = TextAlignmentType.Bottom;
            
            Console.WriteLine("Initial Vertical Alignment: " + shape.TextVerticalAlignment);

            // Cambiar alineación vertical
            if (shape.TextVerticalAlignment == TextAlignmentType.Bottom)
            {
                shape.TextVerticalAlignment = TextAlignmentType.Center;
            }

            Console.WriteLine("Updated Vertical Alignment: " + shape.TextVerticalAlignment);

            // Guarda el libro de trabajo
            workbook.Save("TextVerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


