---
title: "TextEffectFormat.RotatedChars"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextEffectFormat. Si es true, los caracteres en el WordArt especificado se rotan 90 grados respecto a la forma delimitadora del WordArt"
type: docs
url: /es/net/aspose.cells.drawing/texteffectformat/rotatedchars/
---
## TextEffectFormat.RotatedChars property

Si es verdadero, los caracteres en el WordArt especificado se rotan 90 grados respecto a la forma delimitadora del WordArt.

```csharp
public bool RotatedChars { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyRotatedCharsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma con efecto de texto
            Shape shape = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", 
                "Arial", 18, false, false, 0, 0, 100, 100, 200, 50);

            // Obtener el formato de efecto de texto
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // Establecer la propiedad RotatedChars a true
            textEffectFormat.RotatedChars = true;

            // Guarda el libro de trabajo
            workbook.Save("TextEffectFormat_RotatedChars_Output.xlsx");

            // Verificar la propiedad RotatedChars
            Console.WriteLine("RotatedChars property value: " + textEffectFormat.RotatedChars);
        }
    }
}
```

### Ver también

* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


