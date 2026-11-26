---
title: "Класс CharacterBulletValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.Texts.CharacterBulletValue. Представляет символьный маркер"
type: docs
url: /ru/net/aspose.cells.drawing.texts/characterbulletvalue/
---
## CharacterBulletValue class

Представляет символьный маркер.

```csharp
public class CharacterBulletValue : BulletValue
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CharacterBulletValue](characterbulletvalue/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Character](../../aspose.cells.drawing.texts/characterbulletvalue/character/) { get; set; } | Получает и задает символ маркера. |
| override [Type](../../aspose.cells.drawing.texts/characterbulletvalue/type/) { get; } | Получает тип маркера. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassCharacterBulletValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample text";

            TextParagraph paragraph = textbox.TextBody.TextParagraphs[0];
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Percentage;
            paragraph.LineSpace = 3000;

            Bullet bullet = paragraph.Bullet;
            bullet.Type = BulletType.Character;
            ((CharacterBulletValue)bullet.BulletValue).Character = 'v';
            bullet.FontName = "Arial";

            workbook.Save("CharacterBulletValueDemo.xlsx");
        }
    }
}
```

### См. также

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


