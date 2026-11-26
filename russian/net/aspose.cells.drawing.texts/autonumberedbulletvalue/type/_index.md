---
title: "AutoNumberedBulletValue.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AutoNumberedBulletValue. Возвращает тип маркера"
type: docs
url: /ru/net/aspose.cells.drawing.texts/autonumberedbulletvalue/type/
---
## AutoNumberedBulletValue.Type property

Получает тип маркера.

```csharp
public override BulletType Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму для добавления текста с маркерами
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 10, 300, 100);
            var textParagraph = shape.TextBody.TextParagraphs[0];

            // Создать значение автонумерованного маркера
            var bullet = new AutoNumberedBulletValue
            {
                AutonumberScheme = TextAutonumberScheme.AlphaLcParenBoth,
                StartAt = 1
            };

            // Поскольку мы не можем установить BulletValue напрямую, нам потребуется найти другой способ
            // для применения стиля маркера. Это может потребовать использования форматирования текста формы
            // или других доступных методов в API.
            // Для демонстрации мы просто отобразим тип маркера
            Console.WriteLine("Bullet Type: " + bullet.Type);

            // Добавить текст в абзац через текстовое тело формы
            shape.TextBody.Text = "First Item";

            // Добавить еще один абзац с другой схемой нумерации
            // Поскольку мы не можем добавить, мы используем следующий доступный абзац
            var secondParagraph = shape.TextBody.TextParagraphs[1];
            var bullet2 = new AutoNumberedBulletValue
            {
                AutonumberScheme = TextAutonumberScheme.Arabic1Minus,
                StartAt = 1
            };

            // Отобразить тип маркера (только для чтения свойство)
            Console.WriteLine("Second Bullet Type: " + bullet2.Type);

            // Добавить текст во второй абзац
            shape.TextBody.Text += "\nSecond Item";

            // Сохранить книгу, чтобы продемонстрировать эффекты маркеров
            workbook.Save("AutoNumberedBulletDemo.xlsx");
        }
    }

}
```

### См. также

* enum [BulletType](../../bullettype/)
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


