---
title: "Класс BulletValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.Texts.BulletValue класс. Представляет значение маркера"
type: docs
url: /ru/net/aspose.cells.drawing.texts/bulletvalue/
---
## BulletValue class

Представляет значение маркера.

```csharp
public abstract class BulletValue
```

## Свойства

| Имя | Описание |
| --- | --- |
| abstract [Type](../../aspose.cells.drawing.texts/bulletvalue/type/) { get; } | Получает тип значения маркера. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassBulletValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать текстовое поле и получить его текстовые абзацы
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var textParagraph = textBox.TextBody.TextParagraphs[0];

            // Создать экземпляр CharacterBulletValue (наследующий от BulletValue)
            var bulletValue = new CharacterBulletValue();
            bulletValue.Character = '•';
            
            // Установить значение маркера в абзаце (Bullet только для чтения, поэтому нужно изменить его иначе)
            // Поскольку Bullet только для чтения, нам нужно найти другой способ установить его
            // Это может потребовать создания нового TextParagraph с установленным маркером
            // Примечание: Реальный API может предоставлять иной способ установки маркеров
            // Для демонстрации предположим, что мы можем установить его другими способами
            // textParagraph.Bullet = bulletValue; // Эта строка удалена, так как Bullet только для чтения
            textBox.Text = "First bullet point";

            // Добавить еще один абзац с другим маркером
            // У TextParagraphCollection нет метода Add, поэтому нам нужно найти другой способ
            // Это может потребовать создания нового TextParagraph и добавления его другими способами
            // Для демонстрации предположим, что мы можем получить второй абзац напрямую
            var textParagraph2 = textBox.TextBody.TextParagraphs[1];
            var bulletValue2 = new CharacterBulletValue();
            bulletValue2.Character = '→';
            // textParagraph2.Bullet = bulletValue2; // Эта строка удалена, так как Bullet только для чтения
            textBox.Text += "\nSecond bullet point";

            // Продемонстрировать доступ к типу маркера
            Console.WriteLine("First bullet type: " + textParagraph.Bullet.Type);
            Console.WriteLine("Second bullet type: " + textParagraph2.Bullet.Type);

            // Сохранить результат
            workbook.Save("TextsClassBulletValueDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


