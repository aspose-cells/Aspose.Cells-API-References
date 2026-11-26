---
title: "TextEffectFormat.PresetShape"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextEffectFormat. Obtiene y establece el tipo de forma predefinida"
type: docs
url: /es/net/aspose.cells.drawing/texteffectformat/presetshape/
---
## TextEffectFormat.PresetShape property

Obtiene y establece el tipo de forma predefinido.

```csharp
public MsoPresetTextEffectShape PresetShape { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextEffectFormatPropertyPresetShapeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma con efecto de texto
            Shape shape = worksheet.Shapes.AddTextEffect(
                MsoPresetTextEffect.TextEffect1,
                "Sample Text",
                "Arial",
                18,
                false,
                false,
                0,
                0,
                100,
                200,
                0,
                0);

            // Obtener el formato de efecto de texto
            TextEffectFormat textEffectFormat = shape.TextEffect;

            // Establecer y obtener la propiedad PresetShape
            textEffectFormat.PresetShape = MsoPresetTextEffectShape.ArchUpPour;
            Console.WriteLine("PresetShape: " + textEffectFormat.PresetShape);

            // Modificar otras propiedades
            textEffectFormat.Text = "Updated Text";
            textEffectFormat.FontBold = true;
            textEffectFormat.FontSize = 24;

            // Guarda el libro de trabajo
            workbook.Save("TextEffectFormatDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [MsoPresetTextEffectShape](../../msopresettexteffectshape/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


