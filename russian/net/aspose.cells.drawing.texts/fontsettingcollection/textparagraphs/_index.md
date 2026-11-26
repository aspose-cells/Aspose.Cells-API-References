---
title: "FontSettingCollection.TextParagraphs"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FontSettingCollection. Получает все абзацы"
type: docs
url: /ru/net/aspose.cells.drawing.texts/fontsettingcollection/textparagraphs/
---
## FontSettingCollection.TextParagraphs property

Получает все абзацы.

```csharp
public TextParagraphCollection TextParagraphs { get; }
```

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле на лист
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "First paragraph\nSecond paragraph";

            // Получить доступ к первому текстовому абзацу
            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];
            
            // Задать свойства межстрочного интервала
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
            paragraph.LineSpace = 3000; // 300% line spacing

            // Задать свойства маркеров
            Bullet bullet = paragraph.Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Сохраните книгу
            workbook.Save("TextParagraphsDemo.xlsx");
        }
    }
}
```

### См. также

* class [TextParagraphCollection](../../textparagraphcollection/)
* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


