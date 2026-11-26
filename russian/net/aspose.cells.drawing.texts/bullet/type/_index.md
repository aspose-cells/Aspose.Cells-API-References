---
title: "Bullet.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Bullet. Получает и задает тип маркера"
type: docs
url: /ru/net/aspose.cells.drawing.texts/bullet/type/
---
## Bullet.Type property

Получает и задает тип маркера.

```csharp
public BulletType Type { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class BulletPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить текстовое поле
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample text with bullet";

            // Настройте свойства маркера
            Bullet bullet = textbox.TextBody.TextParagraphs[0].Bullet;
            bullet.Type = BulletType.Character; // Demonstrating Type property usage
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Сохраните книгу
            workbook.Save("BulletPropertyTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [BulletType](../../bullettype/)
* class [Bullet](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


