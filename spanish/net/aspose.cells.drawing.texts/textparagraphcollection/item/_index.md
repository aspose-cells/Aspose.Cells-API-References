---
title: "TextParagraphCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextParagraphCollection. Obtiene el objeto TextParagraph en un índice específico"
type: docs
url: /es/net/aspose.cells.drawing.texts/textparagraphcollection/item/
---
## TextParagraphCollection indexer

Obtiene el objeto [`TextParagraph`](../../textparagraph/) en un índice específico.

```csharp
public TextParagraph this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Ejemplos

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

            // Acceder al párrafo usando la propiedad Item
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

### Ver también

* class [TextParagraph](../../textparagraph/)
* class [TextParagraphCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


