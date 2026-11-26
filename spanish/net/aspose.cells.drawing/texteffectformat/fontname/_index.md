---
title: "TextEffectFormat.FontName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextEffectFormat. El nombre de la fuente utilizada en el WordArt"
type: docs
url: /es/net/aspose.cells.drawing/texteffectformat/fontname/
---
## TextEffectFormat.FontName property

El nombre de la fuente utilizada en el WordArt.

```csharp
public string FontName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyFontNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma WordArt
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 0, 0, 100, 100);

            // Establecer y obtener la propiedad FontName
            shape.TextEffect.FontName = "+mn-ea";
            string fontName = shape.TextEffect.FontName;

            // Mostrar el resultado
            Console.WriteLine("Font Name: " + fontName);
        }
    }
}
```

### Ver también

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


