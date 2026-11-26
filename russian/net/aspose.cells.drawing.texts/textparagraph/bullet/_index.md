---
title: "TextParagraph.Bullet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextParagraph. Получает маркер"
type: docs
url: /ru/net/aspose.cells.drawing.texts/textparagraph/bullet/
---
## TextParagraph.Bullet property

Получает маркер.

```csharp
public Bullet Bullet { get; }
```

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            
            // Установить текст и настроить абзац
            textbox.Text = "First Item\nSecond Item";
            textbox.TextBody.TextParagraphs[0].LineSpaceSizeType = LineSpaceSizeType.Percentage;
            textbox.TextBody.TextParagraphs[0].LineSpace = 3000;

            // Настроить маркер для первого абзаца
            Bullet bullet = textbox.TextBody.TextParagraphs[0].Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Сохраните книгу
            workbook.Save("TextParagraphPropertyBulletDemo.xlsx");
        }
    }
}
```

### См. также

* class [Bullet](../../bullet/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


