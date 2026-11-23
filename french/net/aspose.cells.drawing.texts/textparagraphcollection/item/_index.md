---
title: "TextParagraphCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TextParagraphCollection. Obtient l'objet TextParagraph à un indice spécifique"
type: docs
url: /fr/net/aspose.cells.drawing.texts/textparagraphcollection/item/
---
## TextParagraphCollection indexer

Obtient l'objet [`TextParagraph`](../../textparagraph/) à un indice spécifique.

```csharp
public TextParagraph this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Exemples

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

            // Accédez au paragraphe en utilisant la propriété Item
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

### Voir aussi

* class [TextParagraph](../../textparagraph/)
* class [TextParagraphCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


