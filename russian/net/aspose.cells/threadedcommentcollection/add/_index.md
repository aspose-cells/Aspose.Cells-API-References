---
title: "ThreadedCommentCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ThreadedCommentCollection. Добавляет ветвистый комментарий"
type: docs
url: /ru/net/aspose.cells/threadedcommentcollection/add/
---
## ThreadedCommentCollection.Add method

Добавляет цепочный комментарий.

```csharp
public int Add(string text, ThreadedCommentAuthor author)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| текст | String | Текст ветвистого комментария. |
| автор | ThreadedCommentAuthor | Автор ветвистого комментария |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentCollectionMethodAddWithStringThreadedCommentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные для контекста
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Создайте автора ветвистого комментария, используя ThreadedCommentAuthorCollection
                ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
                int authorIndex = authors.Add("John Doe", "john.doe@example.com", "EXAMPLE_PROVIDER");
                ThreadedCommentAuthor author = authors[authorIndex];

                // Получите доступ к коллекции ветвистых комментариев ячейки
                Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
                ThreadedCommentCollection threadedComments = comment.ThreadedComments;

                // Вызовите метод Add с параметрами String и ThreadedCommentAuthor
                int commentIndex = threadedComments.Add("This is a threaded comment", author);

                // Отобразить результат
                Console.WriteLine($"Added threaded comment at index: {commentIndex}");
                Console.WriteLine($"Comment text: {threadedComments[commentIndex].Notes}");
                Console.WriteLine($"Author: {threadedComments[commentIndex].Author.Name}");

                // Сохраните книгу
                workbook.Save("ThreadedCommentAddDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


