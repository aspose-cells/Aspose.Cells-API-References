---
title: "BulletValue.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство BulletValue. Возвращает тип значения маркера"
type: docs
url: /ru/net/aspose.cells.drawing.texts/bulletvalue/type/
---
## BulletValue.Type property

Получает тип значения маркера.

```csharp
public abstract BulletType Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class BulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создать текстовое поле и получить его текстовые абзацы
                var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
                var textParagraph = textBox.TextBody.TextParagraphs[0];

                // Создать значение символного маркера (наследующее от BulletValue)
                var bulletValue = new CharacterBulletValue();
                bulletValue.Character = '•';

                // Отобразите значение свойства Type
                Console.WriteLine("Bullet Type: " + bulletValue.Type);

                // Создать значение графического маркера для отображения другого типа
                var pictureBullet = new PictureBulletValue();
                Console.WriteLine("Picture Bullet Type: " + pictureBullet.Type);

                // Сохраните книгу
                workbook.Save("BulletValueTypeDemo.xlsx");
                Console.WriteLine("Type property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* enum [BulletType](../../bullettype/)
* class [BulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


