---
title: "TextBoxOptions.WrapTextInShape"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxOptions. Especifica el ajuste de texto dentro de una forma. False  No se producirá ajuste en el cuerpo del texto. True  Se producirá ajuste en el cuerpo del texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/textboxoptions/wraptextinshape/
---
## TextBoxOptions.WrapTextInShape property

Especifica el ajuste de texto dentro de una forma. False - No se producirá ajuste en el cuerpo del texto. True - Se producirá ajuste en el cuerpo del texto.

```csharp
public bool WrapTextInShape { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyWrapTextInShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de cuadro de texto con los parámetros correctos
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);

            // Establecer texto que se ajustará dentro de la forma
            textBox.Text = "This is a long text that should wrap within the text box shape boundaries when WrapTextInShape is enabled.";

            // Habilitar el ajuste de texto dentro de la forma
            textBox.TextBoxOptions.WrapTextInShape = true;

            // Guarda el libro de trabajo
            workbook.Save("TextBoxWrapTextDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


