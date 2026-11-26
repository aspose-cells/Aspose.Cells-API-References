---
title: "Comment.Author"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Comment. Получает и задает имя оригинального автора комментария"
type: docs
url: /ru/net/aspose.cells/comment/author/
---
## Comment.Author property

Получает и задает имя оригинального автора комментария

```csharp
public string Author { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyAuthorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарий к ячейке A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Установить автора комментария и заметку
            comment.Author = "Carl.Yang";
            comment.Note = "This is a sample comment";

            // Отобразить автора комментария
            Console.WriteLine("Comment Author: " + comment.Author);
        }
    }
}
```

### См. также

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


