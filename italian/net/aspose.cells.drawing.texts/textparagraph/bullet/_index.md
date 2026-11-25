---
title: "TextParagraph.Bullet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraph. Ottiene il punto elenco"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraph/bullet/
---
## TextParagraph.Bullet property

Ottiene il bullet.

```csharp
public Bullet Bullet { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertyBulletDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            
            // Imposta il testo e configura il paragrafo
            textbox.Text = "First Item\nSecond Item";
            textbox.TextBody.TextParagraphs[0].LineSpaceSizeType = LineSpaceSizeType.Percentage;
            textbox.TextBody.TextParagraphs[0].LineSpace = 3000;

            // Configura il punto elenco per il primo paragrafo
            Bullet bullet = textbox.TextBody.TextParagraphs[0].Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Salva la cartella di lavoro
            workbook.Save("TextParagraphPropertyBulletDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Bullet](../../bullet/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


