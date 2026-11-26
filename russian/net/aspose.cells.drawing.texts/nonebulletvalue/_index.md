---
title: "Класс NoneBulletValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Drawing.Texts.NoneBulletValue класс. Представляет отсутствие маркера"
type: docs
url: /ru/net/aspose.cells.drawing.texts/nonebulletvalue/
---
## NoneBulletValue class

Представляет отсутствие маркера.

```csharp
public class NoneBulletValue : BulletValue
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [NoneBulletValue](nonebulletvalue/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| override [Type](../../aspose.cells.drawing.texts/nonebulletvalue/type/) { get; } | Получает тип значения маркера. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class NoneBulletValueDemo
    {
        public static void NoneBulletValueExample()
        {
            // Создать новую книгу и получить доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавление текста в ячейку
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample text without bullet");

            // Создать TextBox для применения настроек маркера
            Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[worksheet.TextBoxes.Add(2, 1, 100, 400)];
            textBox.Text = "This is a TextBox without bullet points";

            // Создать экземпляр NoneBulletValue
            NoneBulletValue noneBulletValue = new NoneBulletValue();

            // Проверьте тип маркера (должен быть None)
            BulletType bulletType = noneBulletValue.Type;
            Console.WriteLine("Bullet Type: " + bulletType); // Output should be None

            // Сохранить рабочую книгу, чтобы продемонстрировать изменения
            workbook.Save("NoneBulletValueExample.xlsx");
        }
    }
}
```

### См. также

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


