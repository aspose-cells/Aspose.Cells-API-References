---
title: "TextEffectFormat.SetTextEffect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método TextEffectFormat. Establece el efecto de texto predefinido"
type: docs
url: /es/net/aspose.cells.drawing/texteffectformat/settexteffect/
---
## TextEffectFormat.SetTextEffect method

Establece el efecto de texto predefinido.

```csharp
public void SetTextEffect(MsoPresetTextEffect effect)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| efecto | MsoPresetTextEffect | El efecto de texto predefinido. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextEffectFormatMethodSetTextEffectWithMsoPresetTextEffectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para WordArt
            Shape wordArt = worksheet.Shapes.AddTextEffect(MsoPresetTextEffect.TextEffect1, "Sample Text", "Arial", 36, false, false, 0, 0, 0, 0, 100, 100);

            // Obtener el TextEffectFormat de la forma
            TextEffectFormat textEffectFormat = wordArt.TextEffect;

            try
            {
                // Llamar al método SetTextEffect con el parámetro MsoPresetTextEffect
                textEffectFormat.SetTextEffect(MsoPresetTextEffect.TextEffect10);

                // Establecer propiedades adicionales para el WordArt
                textEffectFormat.FontBold = true;
                textEffectFormat.FontItalic = false;
                textEffectFormat.FontSize = 24;

                Console.WriteLine("SetTextEffect method executed successfully with MsoPresetTextEffect.TextEffect10");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextEffect method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("TextEffectFormatMethodSetTextEffectWithMsoPresetTextEffectDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [TextEffectFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


