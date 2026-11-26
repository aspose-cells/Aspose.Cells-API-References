---
title: "ShapeTextAlignment.IsLockedText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeTextAlignment. Indica si la forma está bloqueada cuando la hoja de cálculo está protegida"
type: docs
url: /es/net/aspose.cells.drawing.texts/shapetextalignment/islockedtext/
---
## ShapeTextAlignment.IsLockedText property

Indica si la forma está bloqueada cuando la hoja de cálculo está protegida.

```csharp
public bool IsLockedText { get; set; }
```

### Observaciones

Solo funciona cuando la hoja de cálculo está protegida.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyIsLockedTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            textBox.Text = "Sample Text";

            // Acceder a las propiedades de alineación de texto
            Aspose.Cells.Drawing.Texts.ShapeTextAlignment textAlignment = textBox.TextBody.TextAlignment;

            // Establecer y demostrar la propiedad IsLockedText
            textAlignment.IsLockedText = true;
            Console.WriteLine("Text locked status: " + textAlignment.IsLockedText);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


