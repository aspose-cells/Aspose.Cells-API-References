---
title: "TextParagraph.AlignmentType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextParagraph. Obtiene y establece el tipo de alineación horizontal del texto del párrafo"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/alignmenttype/
---
## TextParagraph.AlignmentType property

Obtiene y establece el tipo de alineación horizontal del texto del párrafo.

```csharp
public TextAlignmentType AlignmentType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertyAlignmentTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una forma de cuadro de texto
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 300, 200, 100);
            textBox.Text = "First Line\nSecond Line\nThird Line";
            
            // Obtener los párrafos de texto
            TextParagraphCollection paragraphs = textBox.TextBody.TextParagraphs;
            
            // Establecer una alineación diferente para cada párrafo
            paragraphs[0].AlignmentType = TextAlignmentType.Center;
            paragraphs[1].AlignmentType = TextAlignmentType.Left;
            paragraphs[2].AlignmentType = TextAlignmentType.Right;
            
            // Guarda el libro de trabajo
            workbook.Save("TextParagraphAlignmentDemo.xlsx");
            
            Console.WriteLine("Text paragraph alignment demo completed successfully.");
        }
    }
}
```

### Ver también

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


