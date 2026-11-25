---
title: "TextParagraph.Children"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraph. Ottiene tutti i run di testo in questo paragrafo. Se questo paragrafo è vuoto restituisce il paragrafo stesso"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/children/
---
## TextParagraph.Children property

Ottiene tutti i run di testo in questo paragrafo. Se questo paragrafo è vuoto, restituisce lo stesso paragrafo.

```csharp
public FontSetting[] Children { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyChildrenDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 200, 100, 200);
            textBox.Text = "First line\nSecond line\nThird line";

            // Ottieni la raccolta di paragrafi di testo
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // Visualizza il numero di elementi figli (run di testo) nel paragrafo
            Console.WriteLine("Number of children (text runs): " + textParagraph.Children.Length);

            // Modifica le impostazioni del carattere di ogni elemento figlio (run di testo)
            foreach (FontSetting child in textParagraph.Children)
            {
                child.Font.Size = 12;
                child.Font.Color = System.Drawing.Color.Blue;
                child.Font.IsBold = true;
            }

            // Aggiungi un'altra riga con formattazione diversa
            textBox.Text += "\nFourth line";
            fontSetting = (FontSetting)textBox.GetCharacters()[textBox.Text.Length - 1];
            textParagraph = (TextParagraph)fontSetting;

            // Visualizza il numero aggiornato di figli
            Console.WriteLine("Updated number of children: " + textParagraph.Children.Length);

            // Salva la cartella di lavoro
            workbook.Save("TextParagraphChildrenDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


