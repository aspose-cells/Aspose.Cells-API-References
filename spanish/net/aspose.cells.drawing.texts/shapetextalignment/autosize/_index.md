---
title: "ShapeTextAlignment.AutoSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeTextAlignment. Indica si el tamaño de la forma se ajusta automáticamente según su contenido"
type: docs
url: /es/net/aspose.cells.drawing.texts/shapetextalignment/autosize/
---
## ShapeTextAlignment.AutoSize property

Indica si el tamaño de la forma se ajusta automáticamente según su contenido.

```csharp
public bool AutoSize { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyAutoSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de cuadro de texto
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 100, 200);
            textBox.Text = "This is a sample text that will demonstrate AutoSize property functionality";

            // Obtener alineación de texto
            ShapeTextAlignment shapeTextAlignment = textBox.TextBody.TextAlignment;

            // Demostrar AutoSize = false (por defecto)
            shapeTextAlignment.AutoSize = false;
            Console.WriteLine("AutoSize false - Fixed size: " + textBox.Width + "x" + textBox.Height);

            // Demostrar AutoSize = true
            shapeTextAlignment.AutoSize = true;
            Console.WriteLine("AutoSize true - Auto sized: " + textBox.Width + "x" + textBox.Height);

            // Guarda el libro de trabajo
            workbook.Save("ShapeTextAlignmentAutoSizeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


