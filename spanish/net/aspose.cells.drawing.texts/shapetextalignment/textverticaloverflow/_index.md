---
title: "ShapeTextAlignment.TextVerticalOverflow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeTextAlignment. Obtiene y establece el tipo de desbordamiento vertical del texto del cuadro de texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/shapetextalignment/textverticaloverflow/
---
## ShapeTextAlignment.TextVerticalOverflow property

Obtiene y establece el tipo de desbordamiento vertical del texto del cuadro de texto.

```csharp
public TextOverflowType TextVerticalOverflow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextVerticalOverflowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);

            // Establecer texto que podría desbordarse verticalmente
            shape.Text = "This is a long text that might overflow vertically if not clipped properly";

            // Obtener la alineación de texto y establecer el desbordamiento vertical a Clip
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;

            // Guarda el libro de trabajo
            workbook.Save("TextVerticalOverflowDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextOverflowType](../../../aspose.cells.drawing/textoverflowtype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


