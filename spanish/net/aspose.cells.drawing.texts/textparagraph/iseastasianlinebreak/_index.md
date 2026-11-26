---
title: "TextParagraph.IsEastAsianLineBreak"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextParagraph. Especifica si una palabra de Asia Oriental puede romperse a la mitad y trasladarse a la siguiente línea sin que se añada un guion"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/iseastasianlinebreak/
---
## TextParagraph.IsEastAsianLineBreak property

Especifica si una palabra de Asia Oriental puede dividirse a la mitad y pasar a la siguiente línea sin que se añada un guion.

```csharp
public bool IsEastAsianLineBreak { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyIsEastAsianLineBreakDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            textBox.Text = "これは東アジアのテキストの例です。This is Latin text example.";

            // Obtén el párrafo de texto del primer párrafo del cuadro de texto
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Mostrar el valor actual de IsEastAsianLineBreak
            Console.WriteLine("Current IsEastAsianLineBreak value: " + paragraph.IsEastAsianLineBreak);

            // Establecer IsEastAsianLineBreak a false (las palabras de Asia Oriental pueden romperse)
            paragraph.IsEastAsianLineBreak = false;
            Console.WriteLine("After setting IsEastAsianLineBreak to false, text may break East Asian words.");

            // Guardar el libro de trabajo con la ruptura de línea de Asia Oriental deshabilitada
            workbook.Save("EastAsianLineBreakDisabled.xlsx");

            // Establecer IsEastAsianLineBreak a true (las palabras de Asia Oriental no se romperán)
            paragraph.IsEastAsianLineBreak = true;
            Console.WriteLine("After setting IsEastAsianLineBreak to true, text won't break East Asian words.");

            // Guardar el libro de trabajo con la ruptura de línea de Asia Oriental habilitada
            workbook.Save("EastAsianLineBreakEnabled.xlsx");
        }
    }
}
```

### Ver también

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


