---
title: "TextParagraph.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraph. Ottiene il tipo di nodo di testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/type/
---
## TextParagraph.Type property

Ottiene il tipo di nodo di testo.

```csharp
public override TextNodeType Type { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro con tutti i parametri richiesti
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 100, 200);
            var textBody = textBox.TextBody;
            textBody.Text = "Sample Text\nSecond Line";

            // Ottieni il primo paragrafo dal corpo del testo
            var paragraphs = textBody.TextParagraphs;
            TextParagraph paragraph = paragraphs[0];

            // Visualizza il valore corrente di Type
            Console.WriteLine("Current TextNodeType: " + paragraph.Type);

            // Dimostra come la proprietà Type influisce sul comportamento
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

            // Salva la cartella di lavoro
            workbook.Save("TextParagraphPropertyTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextNodeType](../../textnodetype/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


