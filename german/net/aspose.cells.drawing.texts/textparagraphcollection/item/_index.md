---
title: "TextParagraphCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextParagraphCollection-Eigenschaft. Gibt das TextParagraph-Objekt an einem bestimmten Index zurück"
type: docs
url: /de/net/aspose.cells.drawing.texts/textparagraphcollection/item/
---
## TextParagraphCollection indexer

Gibt das [`TextParagraph`](../../textparagraph/) Objekt an einem bestimmten Index zurück.

```csharp
public TextParagraph this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index. |

### Beispiele

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

            // Zugriff auf Absatz über die Item-Eigenschaft
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

### Siehe auch

* class [TextParagraph](../../textparagraph/)
* class [TextParagraphCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


