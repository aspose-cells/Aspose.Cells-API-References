---
title: "TextParagraph.IsEastAsianLineBreak"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraph. Specifica se una parola dell'Est asiatico può essere divisa a metà e avvolta alla riga successiva senza aggiungere un trattino"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/iseastasianlinebreak/
---
## TextParagraph.IsEastAsianLineBreak property

Specifica se una parola dell'Est asiatico può essere divisa a metà e spostata alla riga successiva senza aggiungere un trattino.

```csharp
public bool IsEastAsianLineBreak { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            textBox.Text = "これは東アジアのテキストの例です。This is Latin text example.";

            // Ottieni il paragrafo di testo dal primo paragrafo della casella di testo
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // Visualizza il valore corrente di IsEastAsianLineBreak
            Console.WriteLine("Current IsEastAsianLineBreak value: " + paragraph.IsEastAsianLineBreak);

            // Imposta IsEastAsianLineBreak su false (le parole dell'Est asiatico possono essere divise)
            paragraph.IsEastAsianLineBreak = false;
            Console.WriteLine("After setting IsEastAsianLineBreak to false, text may break East Asian words.");

            // Salva la cartella di lavoro con interruzione di riga dell'Est asiatico disabilitata
            workbook.Save("EastAsianLineBreakDisabled.xlsx");

            // Imposta IsEastAsianLineBreak su true (le parole dell'Est asiatico non saranno divise)
            paragraph.IsEastAsianLineBreak = true;
            Console.WriteLine("After setting IsEastAsianLineBreak to true, text won't break East Asian words.");

            // Salva la cartella di lavoro con interruzione di riga dell'Est asiatico abilitata
            workbook.Save("EastAsianLineBreakEnabled.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


