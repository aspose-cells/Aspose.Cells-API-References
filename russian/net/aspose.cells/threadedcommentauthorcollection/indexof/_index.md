---
title: "ThreadedCommentAuthorCollection.IndexOf"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ThreadedCommentAuthorCollection. Возвращает индекс объекта ThreadedCommentAuthor"
type: docs
url: /ru/net/aspose.cells/threadedcommentauthorcollection/indexof/
---
## ThreadedCommentAuthorCollection.IndexOf method

Возвращает индекс объекта ThreadedCommentAuthor

```csharp
public int IndexOf(ThreadedCommentAuthor author)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| автор | ThreadedCommentAuthor | Объект ThreadedCommentAuthor |

### Возвращаемое значение

Индекс в коллекции ThreadedCommentAuthor

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorCollectionMethodIndexOfWithThreadedCommentAuthorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите коллекцию авторов ветвящихся комментариев
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

            // Добавьте авторов в коллекцию
            int johnIndex = authors.Add("John Doe", "john.doe", "provider1");
            int janeIndex = authors.Add("Jane Smith", "jane.smith", "provider2");

            // Получите объекты авторов
            ThreadedCommentAuthor johnAuthor = authors[johnIndex];
            ThreadedCommentAuthor janeAuthor = authors[janeIndex];

            try
            {
                // Вызовите метод IndexOf, чтобы найти позицию Джейн Смит
                int foundIndex = authors.IndexOf(janeAuthor);
                
                // Отобразить результат
                Console.WriteLine($"Author '{janeAuthor.Name}' found at index: {foundIndex}");

                // Проверьте, что результат соответствует ожидаемому индексу
                if (foundIndex == janeIndex)
                {
                    Console.WriteLine("IndexOf result matches the expected index");
                }
                else
                {
                    Console.WriteLine("IndexOf result does not match the expected index");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IndexOf method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("ThreadedCommentAuthorIndexOfDemo.xlsx");
        }
    }
}
```

### См. также

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


