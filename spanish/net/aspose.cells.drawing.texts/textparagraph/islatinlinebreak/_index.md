---
title: "TextParagraph.IsLatinLineBreak"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de TextParagraph. Especifica si una palabra latina puede dividirse a la mitad y pasar a la siguiente línea sin que se añada un guion"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/islatinlinebreak/
---
## TextParagraph.IsLatinLineBreak property

Especifica si una palabra latina puede dividirse a la mitad y pasar a la siguiente línea sin que se añada un guion.

```csharp
public bool IsLatinLineBreak { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsLatinLineBreakDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añade un cuadro de texto a la hoja de cálculo (parámetros corregidos para incluir la altura)
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 300, 200, 100);
            textBox.Text = "This is a long Latin text that will demonstrate line breaking behavior when IsLatinLineBreak is set to different values.";

            // Obtén el párrafo de texto del cuadro de texto (se añadió una conversión explícita)
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = ((TextParagraph)fontSetting);

            // Muestra el valor actual de IsLatinLineBreak
            Console.WriteLine("Current IsLatinLineBreak value: " + textParagraph.IsLatinLineBreak);

            // Establece IsLatinLineBreak a false (las palabras latinas no se dividirán al final de la línea)
            textParagraph.IsLatinLineBreak = false;
            Console.WriteLine("Set IsLatinLineBreak to false - Latin words won't break at line end");
            workbook.Save("LatinLineBreakDisabled.xlsx");

            // Establece IsLatinLineBreak a true (las palabras latinas pueden dividirse al final de la línea)
            textParagraph.IsLatinLineBreak = true;
            Console.WriteLine("Set IsLatinLineBreak to true - Latin words can break at line end");
            workbook.Save("LatinLineBreakEnabled.xlsx");
        }
    }
}
```

### Ver también

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


