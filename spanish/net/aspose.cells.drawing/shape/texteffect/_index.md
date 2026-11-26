---
title: "Shape.TextEffect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Devuelve un objeto TextEffectFormat que contiene propiedades de formato de efecto de texto para la forma especificada. Se aplica a objetos Shape que representan WordArt"
type: docs
url: /es/net/aspose.cells.drawing/shape/texteffect/
---
## Shape.TextEffect property

Devuelve un objeto TextEffectFormat que contiene propiedades de formato de efectos de texto para la forma especificada. Se aplica a objetos Shape que representan WordArt.

```csharp
public TextEffectFormat TextEffect { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextEffectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma WordArt con los parámetros correctos
            Shape shape = worksheet.Shapes.AddWordArt(PresetWordArtStyle.WordArtStyle1, "Sample Text", 10, 10, 200, 50, 0, 0);

            // Verificar si es WordArt y acceder a las propiedades TextEffect
            if (shape.IsWordArt)
            {
                TextEffectFormat textEffectFormat = shape.TextEffect;
                textEffectFormat.FontBold = true;
                textEffectFormat.FontItalic = true;
                textEffectFormat.FontName = "Arial";
                textEffectFormat.FontSize = 14;
            }

            // Guarda el libro de trabajo
            workbook.Save("TextEffectDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextEffectFormat](../../texteffectformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


