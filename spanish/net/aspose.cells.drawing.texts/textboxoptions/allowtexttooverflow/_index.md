---
title: "TextBoxOptions.AllowTextToOverflow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxOptions. Si permite que el texto desborde la forma"
type: docs
url: /es/net/aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/
---
## TextBoxOptions.AllowTextToOverflow property

Si permite que el texto desborde la forma.

```csharp
public bool AllowTextToOverflow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyAllowTextToOverflowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);

            // Establecer texto que podría desbordarse
            textBox.Text = "This is a long text that might overflow the text box boundaries if AllowTextToOverflow is false";

            // Habilitar desbordamiento de texto
            textBox.TextBoxOptions.AllowTextToOverflow = true;

            // Guarda el libro de trabajo
            workbook.Save("TextBoxAllowTextToOverflowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


