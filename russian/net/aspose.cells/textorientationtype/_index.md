---
title: "Перечисление TextOrientationType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.TextOrientationType. Перечисляет типы ориентации текста"
type: docs
url: /ru/net/aspose.cells/textorientationtype/
---
## TextOrientationType enumeration

Перечисляет типы ориентации текста.

```csharp
public enum TextOrientationType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| ClockWise | `0` | Поворачивает текст на 90 градусов по часовой стрелке. |
| CounterClockWise | `1` | Поворачивает текст на 90 градусов против часовой стрелки. |
| NoRotation | `2` | Представляет значение по умолчанию. |
| TopToBottom | `3` | Отображает текст сверху вниз в ячейке. Сложенный текст. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextOrientationTypeDemo
    {
        public static void TextOrientationTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Hello, Aspose!");
            worksheet.Cells["A2"].PutValue("This is a test comment.");

            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add(0, 0);
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a comment with text orientation.";

            // Установить различные типы ориентации текста для комментария
            comment.TextOrientationType = TextOrientationType.ClockWise;
            Console.WriteLine("Text Orientation: ClockWise");

            // Сохраните книгу
            workbook.Save("TextOrientationTypeExample_ClockWise.xlsx");

            // Изменить ориентацию текста на CounterClockWise
            comment.TextOrientationType = TextOrientationType.CounterClockWise;
            Console.WriteLine("Text Orientation: CounterClockWise");

            // Сохраните книгу
            workbook.Save("TextOrientationTypeExample_CounterClockWise.xlsx");

            // Изменить ориентацию текста на NoRotation
            comment.TextOrientationType = TextOrientationType.NoRotation;
            Console.WriteLine("Text Orientation: NoRotation");

            // Сохраните книгу
            workbook.Save("TextOrientationTypeExample_NoRotation.xlsx");

            // Изменить ориентацию текста на TopToBottom
            comment.TextOrientationType = TextOrientationType.TopToBottom;
            Console.WriteLine("Text Orientation: TopToBottom");

            // Сохраните книгу
            workbook.Save("TextOrientationTypeExample_TopToBottom.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


