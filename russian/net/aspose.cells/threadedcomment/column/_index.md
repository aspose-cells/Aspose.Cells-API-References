---
title: "ThreadedComment.Column"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreadedComment. Возвращает индекс столбца комментария"
type: docs
url: /ru/net/aspose.cells/threadedcomment/column/
---
## ThreadedComment.Column property

Получает индекс столбца комментария.

```csharp
public int Column { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Сначала создайте автора ветвленного комментария
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                
                // Добавьте цепочный комментарий в ячейку A1 (строка 0, столбец 0)
                int commentRow = 0;
                int commentColumn = 0;
                worksheet.Comments.AddThreadedComment(commentRow, commentColumn, "Sample comment text", author);
                
                // Получите первый цепочный комментарий
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];
                
                // Отобразите значение свойства Column (только для чтения)
                Console.WriteLine("Threaded comment column index: " + comment.Column);
                
                // Проверьте, что индекс столбца соответствует месту, где мы разместили комментарий
                if (comment.Column == commentColumn)
                {
                    Console.WriteLine("Comment is correctly placed in column " + commentColumn);
                }
                
                // Сохраните книгу
                workbook.Save("ThreadedCommentColumnDemo.xlsx");
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


