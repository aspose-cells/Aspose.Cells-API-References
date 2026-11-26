---
title: "Перечисление BulletType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.Texts.BulletType enum. Представляет тип маркера."
type: docs
url: /ru/net/aspose.cells.drawing.texts/bullettype/
---
## BulletType enumeration

Представляет тип маркера.

```csharp
public enum BulletType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Без маркера. |
| Character | `1` | Символьный маркер. |
| Picture | `2` | Маркер изображения. |
| AutoNumbered | `3` | Автоматический нумерованный маркер. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassBulletTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте TextBox и задайте текст.
            TextBox textBox = worksheet.TextBoxes[worksheet.TextBoxes.Add(2, 1, 100, 400)];
            textBox.Text = "Sample text with bullet type demonstration";

            // Создать параметры маркеров
            NoneBulletValue noneBullet = new NoneBulletValue();
            BulletType bulletType = noneBullet.Type;

            // Применить настройки маркеров к абзацам текста
            foreach (TextParagraph paragraph in textBox.TextBody.TextParagraphs)
            {
                paragraph.Bullet.Type = bulletType;
            }

            Console.WriteLine("Bullet Type applied: " + bulletType);
            workbook.Save("BulletTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


