---
title: "TextParagraphCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextParagraphCollection. Ottiene l'oggetto TextParagraph a un indice specifico"
type: docs
url: /it/net/aspose.cells.drawing.texts/textparagraphcollection/item/
---
## TextParagraphCollection indexer

Ottiene l'oggetto [`TextParagraph`](../../textparagraph/) a un indice specifico.

```csharp
public TextParagraph this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox0 = worksheet.TextBoxes[textboxIndex];
            textbox0.Text = "Sample text";

            // Accedi al paragrafo usando la proprietà Item
            TextParagraph paragraph = textbox0.TextBody.TextParagraphs[0];
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
            paragraph.LineSpace = 3000;

            Bullet bullet = paragraph.Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = 'v';
            bullet.FontName = "Arial";

            workbook.Save("TextParagraphCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TextParagraph](../../textparagraph/)
* class [TextParagraphCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


