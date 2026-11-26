---
title: "Comment.TextOrientationType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Получает и задает тип ориентации текста комментария"
type: docs
url: /ru/net/aspose.cells/comment/textorientationtype/
---
## Comment.TextOrientationType property

Получает и задает тип ориентации текста в комментарии.

```csharp
public TextOrientationType TextOrientationType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextOrientationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // Установите начальную ориентацию в NoRotation
            comment.TextOrientationType = TextOrientationType.NoRotation;
            Console.WriteLine("Initial orientation: " + comment.TextOrientationType);

            // Изменить ориентацию на TopToBottom, если сейчас NoRotation
            if (comment.TextOrientationType == TextOrientationType.NoRotation)
            {
                comment.TextOrientationType = TextOrientationType.TopToBottom;
                Console.WriteLine("Changed orientation to: " + comment.TextOrientationType);
            }

            // Сохраните книгу
            workbook.Save("CommentOrientationDemo.xlsx");
        }
    }
}
```

### См. также

* enum [TextOrientationType](../../textorientationtype/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


