---
title: "Shape.TextHorizontalOverflow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece el tipo de desbordamiento horizontal del texto de la forma que contiene texto"
type: docs
url: /es/net/aspose.cells.drawing/shape/texthorizontaloverflow/
---
## Shape.TextHorizontalOverflow property

Obtiene y establece el tipo de desbordamiento horizontal del texto de la forma que contiene texto.

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
    public class ShapePropertyTextHorizontalOverflowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de cuadro de texto con los parámetros correctos
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            textBox.Text = "This is a long text that will demonstrate text horizontal overflow functionality";

            // Establecer el tipo de desbordamiento inicial a Clip
            textBox.TextHorizontalOverflow = TextOverflowType.Clip;
            Console.WriteLine("TextHorizontalOverflow set to Clip (text will be clipped)");

            // Cambiar el tipo de desbordamiento a Overflow
            textBox.TextHorizontalOverflow = TextOverflowType.Overflow;
            Console.WriteLine("TextHorizontalOverflow changed to Overflow (text will overflow)");

            // Guarda el libro de trabajo
            workbook.Save("TextHorizontalOverflowDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextOverflowType](../../textoverflowtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


