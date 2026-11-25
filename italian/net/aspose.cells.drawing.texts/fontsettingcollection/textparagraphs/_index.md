---
title: "FontSettingCollection.TextParagraphs"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FontSettingCollection. Ottiene tutti i paragrafi"
type: docs
url: /it/net/aspose.cells.drawing.texts/fontsettingcollection/textparagraphs/
---
## FontSettingCollection.TextParagraphs property

Ottiene tutti i paragrafi.

```csharp
public TextParagraphCollection TextParagraphs { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionPropertyTextParagraphsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "First paragraph\nSecond paragraph";

            // Accedi al primo paragrafo di testo
            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];
            
            // Imposta le proprietà dell'interlinea
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
            paragraph.LineSpace = 3000; // 300% line spacing

            // Imposta le proprietà dei punti elenco
            Bullet bullet = paragraph.Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Salva la cartella di lavoro
            workbook.Save("TextParagraphsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextParagraphCollection](../../textparagraphcollection/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


