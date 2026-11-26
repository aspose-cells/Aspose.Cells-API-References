---
title: "Clase TextEffectFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.TextEffectFormat. Contiene propiedades y métodos que se aplican a objetos WordArt"
type: docs
url: /es/net/aspose.cells.drawing/texteffectformat/
---
## TextEffectFormat class

Contiene propiedades y métodos que se aplican a objetos WordArt.

```csharp
public class TextEffectFormat
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FontBold](../../aspose.cells.drawing/texteffectformat/fontbold/) { get; set; } | Indica si la fuente está en negrita. |
| [FontItalic](../../aspose.cells.drawing/texteffectformat/fontitalic/) { get; set; } | Indica si la fuente está en cursiva. |
| [FontName](../../aspose.cells.drawing/texteffectformat/fontname/) { get; set; } | El nombre de la fuente utilizada en el WordArt. |
| [FontSize](../../aspose.cells.drawing/texteffectformat/fontsize/) { get; set; } | El tamaño (en puntos) de la fuente utilizada en el WordArt. |
| [PresetShape](../../aspose.cells.drawing/texteffectformat/presetshape/) { get; set; } | Obtiene y establece el tipo de forma predefinido. |
| [RotatedChars](../../aspose.cells.drawing/texteffectformat/rotatedchars/) { get; set; } | Si es verdadero, los caracteres en el WordArt especificado se rotan 90 grados respecto a la forma delimitadora del WordArt. |
| [Text](../../aspose.cells.drawing/texteffectformat/text/) { get; set; } | El texto en el WordArt. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetTextEffect](../../aspose.cells.drawing/texteffectformat/settexteffect/)(MsoPresetTextEffect) | Establece el efecto de texto predefinido. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTextEffectFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            
            // Agregar forma de efecto de texto
            shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
            
            // Modificar efecto de texto
            TextEffectFormat textEffectFormat = shapes[0].TextEffect;
            textEffectFormat.SetTextEffect(MsoPresetTextEffect.TextEffect10);
            
            // Guarda el libro de trabajo
            workbook.Save("TextEffectDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


