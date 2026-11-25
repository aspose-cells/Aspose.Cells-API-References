---
title: "TextParagraph.IsHangingPunctuation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraph. Specifica se la punteggiatura deve essere forzatamente posizionata sulla stessa riga di testo o spostata su una riga diversa"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/ishangingpunctuation/
---
## TextParagraph.IsHangingPunctuation property

Specifica se la punteggiatura deve essere forzatamente posizionata su una riga di testo o spostata su una riga diversa.

```csharp
public bool IsHangingPunctuation { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro (corretto aggiungendo il parametro altezza)
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 200, 100, 200, 100);
            textBox.Text = "This is a sample text with punctuation: \"Hello, world!\"";

            // Ottieni il paragrafo di testo dalla casella di testo (corretto mediante cast a TextParagraph)
            FontSetting fontSetting = (FontSetting)textBox.GetCharacters()[0];
            TextParagraph textParagraph = (TextParagraph)fontSetting;

            // Visualizza il valore corrente di IsHangingPunctuation
            Console.WriteLine("Current IsHangingPunctuation value: " + textParagraph.IsHangingPunctuation);

            // Imposta IsHangingPunctuation su true
            textParagraph.IsHangingPunctuation = true;
            Console.WriteLine("IsHangingPunctuation set to: " + textParagraph.IsHangingPunctuation);

            // Imposta IsHangingPunctuation su false
            textParagraph.IsHangingPunctuation = false;
            Console.WriteLine("IsHangingPunctuation set to: " + textParagraph.IsHangingPunctuation);

            // Salva la cartella di lavoro per vedere gli effetti (è necessaria un'ispezione visiva)
            workbook.Save("TextParagraphPropertyIsHangingPunctuationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


