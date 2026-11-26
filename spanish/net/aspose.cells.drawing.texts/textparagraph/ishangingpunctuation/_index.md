---
title: "TextParagraph.IsHangingPunctuation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de TextParagraph. Especifica si la puntuación debe colocarse obligatoriamente en la misma línea de texto o en una línea diferente"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/ishangingpunctuation/
---
## TextParagraph.IsHangingPunctuation property

Especifica si la puntuación debe disponerse forzosamente en una línea de texto o colocarse en una línea de texto diferente.

```csharp
public bool IsHangingPunctuation { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsHangingPunctuationDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añade un cuadro de texto a la hoja de cálculo (corregido añadiendo el parámetro de altura)
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 200, 100, 200, 100);
            textBox.Text = "This is a sample text with punctuation: \"Hello, world!\"";

            // Obtén el párrafo de texto del cuadro de texto (corregido mediante conversión a TextParagraph)
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // Muestra el valor actual de IsHangingPunctuation
            Console.WriteLine("Current IsHangingPunctuation value: " + textParagraph.IsHangingPunctuation);

            // Establece IsHangingPunctuation a true
            textParagraph.IsHangingPunctuation = true;
            Console.WriteLine("IsHangingPunctuation set to: " + textParagraph.IsHangingPunctuation);

            // Establece IsHangingPunctuation a false
            textParagraph.IsHangingPunctuation = false;
            Console.WriteLine("IsHangingPunctuation set to: " + textParagraph.IsHangingPunctuation);

            // Guarda el libro de trabajo para ver los efectos (se requiere inspección visual)
            workbook.Save("TextParagraphPropertyIsHangingPunctuationDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


