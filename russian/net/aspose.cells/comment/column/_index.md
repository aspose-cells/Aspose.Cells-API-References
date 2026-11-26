---
title: "Comment.Column"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Получает индекс столбца комментария"
type: docs
url: /ru/net/aspose.cells/comment/column/
---
## Comment.Column property

Получает индекс столбца комментария.

```csharp
public int Column { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий в ячейку B5 (индекс столбца 1)
            int commentRow = 4;
            int commentColumn = 1;
            Comment comment = worksheet.Comments[worksheet.Comments.Add(commentRow, commentColumn)];

            // Установить текст комментария
            comment.Note = "This is a sample comment";

            // Продемонстрировать использование свойства Column
            Console.WriteLine("Comment is in column: " + comment.Column);

            // Проверьте, что индекс столбца соответствует месту его размещения
            if (comment.Column == commentColumn)
            {
                Console.WriteLine("Column property correctly returns the comment's column index");
            }
        }
    }
}
```

### См. также

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


