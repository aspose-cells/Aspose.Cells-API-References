---
title: "ThreadedComment.Author"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreadedComment. Получает автора комментария"
type: docs
url: /ru/net/aspose.cells/threadedcomment/author/
---
## ThreadedComment.Author property

Получает автора комментария.

```csharp
public ThreadedCommentAuthor Author { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyAuthorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Получите автора цепочного комментария по умолчанию из рабочей книги
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                author.Name = "John Doe";
                author.UserId = "john.doe@example.com";

                // Добавьте цепочный комментарий в ячейку A1 (строка 0, столбец 0)
                worksheet.Comments.AddThreadedComment(0, 0, "Sample comment", author);

                // Получите первый цепочный комментарий
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];

                // Отобразите значение свойства Author (операция чтения)
                Console.WriteLine("Author Name: " + comment.Author.Name);
                Console.WriteLine("Author UserId: " + comment.Author.UserId);
                Console.WriteLine("Author ProviderId: " + comment.Author.ProviderId);

                // Продемонстрируйте установку свойства Author (поскольку оно доступно для чтения и записи)
                ThreadedCommentAuthor newAuthor = workbook.Worksheets.ThreadedCommentAuthors[0];
                newAuthor.Name = "Jane Smith";
                newAuthor.UserId = "jane.smith@example.com";
                comment.Author = newAuthor;

                // Отобразите обновлённое значение свойства Author
                Console.WriteLine("Updated Author Name: " + comment.Author.Name);
                Console.WriteLine("Updated Author UserId: " + comment.Author.UserId);

                // Сохраните книгу
                workbook.Save("ThreadedCommentAuthorDemo.xlsx");
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

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


