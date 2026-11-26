---
title: "ShapeTextAlignment.IsTextWrapped"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeTextAlignment. Obtiene o establece el tipo de ajuste de texto de la forma que contiene texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/shapetextalignment/istextwrapped/
---
## ShapeTextAlignment.IsTextWrapped property

Obtiene o establece el tipo de ajuste de texto de la forma que contiene texto.

```csharp
public bool IsTextWrapped { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Establecer texto de la forma
            shape.Text = "This is a long text that should be wrapped when IsTextWrapped is set to true";

            // Obtener la alineación de texto y establecer IsTextWrapped
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            shapeTextAlignment.IsTextWrapped = true;

            // Guarda el libro de trabajo
            workbook.Save("ShapeTextWrappingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


