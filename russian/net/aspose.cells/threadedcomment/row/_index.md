---
title: "ThreadedComment.Row"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreadedComment. Получает индекс строки комментария"
type: docs
url: /ru/net/aspose.cells/threadedcomment/row/
---
## ThreadedComment.Row property

Получает индекс строки комментария.

```csharp
public int Row { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Создайте автора цепочного комментария
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                author.Name = "Test Author";
                author.UserId = "test@example.com";
                
                // Добавьте цепочный комментарий в ячейку B2 (строка 1, столбец 1)
                worksheet.Comments.AddThreadedComment(1, 1, "Sample threaded comment", author);
                
                // Получите первый цепочный комментарий
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];
                
                // Отобразите значение свойства Row (только для чтения)
                Console.WriteLine("Threaded comment row index: " + comment.Row);
                
                // Проверьте, что индекс строки соответствует месту размещения комментария
                if (comment.Row == 1)
                {
                    Console.WriteLine("Comment is correctly placed in row 1");
                }
                
                // Сохраните книгу
                workbook.Save("ThreadedCommentRowDemo.xlsx");
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

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


