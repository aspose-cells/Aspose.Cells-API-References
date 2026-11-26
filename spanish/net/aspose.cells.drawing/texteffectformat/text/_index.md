---
title: "TextEffectFormat.Text"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextEffectFormat. El texto en el WordArt"
type: docs
url: /es/net/aspose.cells.drawing/texteffectformat/text/
---
## TextEffectFormat.Text property

El texto en el WordArt.

```csharp
public string Text { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar una forma de efecto de texto y establecer su texto
            Shape shape = sheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 14, false, false, 0, 0, 0, 0, 100, 100);

            // Acceder y modificar la propiedad de texto del efecto de texto
            shape.TextEffect.Text = "Updated Text";

            // Verificar que el texto se haya actualizado
            Console.WriteLine("Text Effect Content: " + shape.TextEffect.Text);
        }
    }
}
```

### Ver también

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


