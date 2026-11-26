---
title: "TextBoxOptions.ResizeToFitText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxOptions. Indica si se debe cambiar el tamaño de la forma para ajustarse al texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/textboxoptions/resizetofittext/
---
## TextBoxOptions.ResizeToFitText property

Indica si redimensionar la forma para ajustarse al texto

```csharp
public bool ResizeToFitText { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyResizeToFitTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un cuadro de texto con los parámetros correctos
            Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(1, 1, 100, 100, 200, 50);
            textBox.Text = "This is a sample text that will make the text box resize to fit";

            // Acceder a TextBoxOptions correctamente
            textBox.TextBoxOptions.ResizeToFitText = true;

            // Guarda el libro de trabajo
            workbook.Save("TextBoxResizeToFitTextDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


