---
title: "ThreadedComment.Notes"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreadedComment. Получает и задает текст комментария"
type: docs
url: /ru/net/aspose.cells/threadedcomment/notes/
---
## ThreadedComment.Notes property

Получает и задаёт текст комментария.

```csharp
public string Notes { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentPropertyNotesDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создайте или получите автора цепочного комментария
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors["User1"];
                author.Name = "User1";

                // Добавьте цепочный комментарий в ячейку A1 (строка 0, столбец 0) с начальным текстом
                worksheet.Comments.AddThreadedComment(0, 0, "Initial comment text", author);

                // Получите только что добавленный цепочный комментарий
                ThreadedComment threadedComment = worksheet.Comments[0].ThreadedComments[0];

                // Обновите свойство Notes (текст комментария)
                threadedComment.Notes = "Updated comment notes";

                // Прочитайте и отобразите значение свойства Notes
                Console.WriteLine("Threaded comment Notes: " + threadedComment.Notes);

                // Сохраните книгу (необязательно)
                workbook.Save("ThreadedCommentNotesDemo.xlsx");
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


