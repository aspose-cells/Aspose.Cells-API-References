---
title: "Shape.IsRichText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Indica si el texto es texto enriquecido o no"
type: docs
url: /es/net/aspose.cells.drawing/shape/isrichtext/
---
## Shape.IsRichText property

Indica si el texto es texto enriquecido o no.

```csharp
public bool IsRichText { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsRichTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una forma con texto
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "This is <b>rich</b> text";

            // Verifica si el texto es texto enriquecido
            if (shape.IsRichText)
            {
                Console.WriteLine("The text is rich text.");
            }
            else
            {
                Console.WriteLine("The text is not rich text.");
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


