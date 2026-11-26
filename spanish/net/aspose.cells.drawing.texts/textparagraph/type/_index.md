---
title: "TextParagraph.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextParagraph. Obtiene el tipo de nodo de texto"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraph/type/
---
## TextParagraph.Type property

Obtiene el tipo de nodo de texto.

```csharp
public override TextNodeType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de texto a la hoja de cálculo con todos los parámetros requeridos
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 100, 200);
            var textBody = textBox.TextBody;
            textBody.Text = "Sample Text\nSecond Line";

            // Obtener el primer párrafo del cuerpo de texto
            var paragraphs = textBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[0];

            // Mostrar el valor actual de Type
            Console.WriteLine("Current TextNodeType: " + paragraph.Type);

            // Demostrar cómo la propiedad Type afecta el comportamiento
            if (paragraph.Type == TextNodeType.TextParagraph)
            {
                Console.WriteLine("This is a text paragraph node");
                Console.WriteLine("You can access paragraph-specific properties like:");
                Console.WriteLine("AlignmentType: " + paragraph.AlignmentType);
                Console.WriteLine("LineSpace: " + paragraph.LineSpace);
            }
            else if (paragraph.Type == TextNodeType.TextRun)
            {
                Console.WriteLine("This is a simple text run node");
            }
            else if (paragraph.Type == TextNodeType.Equation)
            {
                Console.WriteLine("This is an equation node");
            }

            // Guarda el libro de trabajo
            workbook.Save("TextParagraphPropertyTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextNodeType](../../textnodetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


