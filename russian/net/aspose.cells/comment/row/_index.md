---
title: "Comment.Row"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Получает индекс строки комментария"
type: docs
url: /ru/net/aspose.cells/comment/row/
---
## Comment.Row property

Получает индекс строки комментария.

```csharp
public int Row { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";

            // Получить и отобразить индекс строки комментируемой ячейки
            int row = comment1.Row;
            Console.WriteLine("The comment is in row: " + row);

            // Добавить еще один комментарий в ячейку B3
            commentIndex = worksheet.Comments.Add("B3");
            Comment comment2 = worksheet.Comments[commentIndex];
            comment2.Note = "Another comment";

            // Отобразить индекс строки второго комментария
            Console.WriteLine("Second comment is in row: " + comment2.Row);
        }
    }
}
```

### См. также

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


