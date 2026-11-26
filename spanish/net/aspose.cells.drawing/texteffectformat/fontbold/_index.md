---
title: "TextEffectFormat.FontBold"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextEffectFormat. Indica si la fuente está en negrita"
type: docs
url: /es/net/aspose.cells.drawing/texteffectformat/fontbold/
---
## TextEffectFormat.FontBold property

Indica si la fuente está en negrita.

```csharp
public bool FontBold { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontBoldDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de cuadro de texto (devuelve el objeto TextBox directamente)
            TextBox textbox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 200, 100);
            textbox.Text = "Sample Text";

            // Obtener el formato de efecto de texto
            TextEffectFormat effFormat = textbox.TextEffect;

            // Establecer propiedades de fuente incluyendo negrita
            effFormat.FontName = "Arial";
            effFormat.FontBold = true;
            effFormat.FontItalic = false;
            effFormat.FontSize = 14;

            // Guarda el libro de trabajo
            workbook.Save("TextEffectFormatFontBoldDemo.xlsx");

            Console.WriteLine("Text effect format with bold font applied successfully.");
        }
    }
}
```

### Ver también

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


