---
title: "TextEffectFormat.FontItalic"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextEffectFormat. Indica si la fuente está en cursiva"
type: docs
url: /es/net/aspose.cells.drawing/texteffectformat/fontitalic/
---
## TextEffectFormat.FontItalic property

Indica si la fuente está en cursiva.

```csharp
public bool FontItalic { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontItalicDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma con efecto de texto
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 0, 0, 100, 100);

            // Obtener el formato de efecto de texto
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // Establecer FontItalic en true
            textEffectFormat.FontItalic = true;
            Console.WriteLine("FontItalic after setting to true: " + textEffectFormat.FontItalic);

            // Establecer FontItalic en false
            textEffectFormat.FontItalic = false;
            Console.WriteLine("FontItalic after setting to false: " + textEffectFormat.FontItalic);

            // Guarda el libro de trabajo
            workbook.Save("TextEffectFormatFontItalicDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


