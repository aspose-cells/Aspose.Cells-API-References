---
title: "Класс Bullet"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.Texts.Bullet класс. Представляет маркеры, которые следует применять к абзацу"
type: docs
url: /ru/net/aspose.cells.drawing.texts/bullet/
---
## Bullet class

Представляет маркеры, которые должны применяться к абзацу.

```csharp
public class Bullet
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BulletValue](../../aspose.cells.drawing.texts/bullet/bulletvalue/) { get; } | Получает значение маркера. |
| [FontName](../../aspose.cells.drawing.texts/bullet/fontname/) { get; set; } | Получает и задает имя шрифта. |
| [Type](../../aspose.cells.drawing.texts/bullet/type/) { get; set; } | Получает и задает тип маркера. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassBulletDemo
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

            workbook.Save("TextsClassBulletDemo_Output.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


