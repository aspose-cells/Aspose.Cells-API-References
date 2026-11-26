---
title: "ShapeTextAlignment.TextHorizontalOverflow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeTextAlignment. Obtiene y establece el tipo de desbordamiento horizontal del texto del cuadro de texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/shapetextalignment/texthorizontaloverflow/
---
## ShapeTextAlignment.TextHorizontalOverflow property

Obtiene y establece el tipo de desbordamiento horizontal del texto del cuadro de texto.

```csharp
public TextOverflowType TextHorizontalOverflow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextHorizontalOverflowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de cuadro de texto
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 50);
            textBox.Text = "This is a long text that demonstrates horizontal overflow behavior";

            // Establecer el desbordamiento horizontal a Clip
            textBox.TextBody.TextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;

            // Guarda el libro de trabajo
            workbook.Save("TextHorizontalOverflowDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextOverflowType](../../../aspose.cells.drawing/textoverflowtype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


