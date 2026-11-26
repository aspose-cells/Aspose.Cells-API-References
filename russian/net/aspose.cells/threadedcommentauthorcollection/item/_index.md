---
title: "ThreadedCommentAuthorCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreadedCommentAuthorCollection. Возвращает человека, который создает ветвящиеся комментарии"
type: docs
url: /ru/net/aspose.cells/threadedcommentauthorcollection/item/
---
## ThreadedCommentAuthorCollection indexer (1 of 2)

Возвращает человека, который создает ветвящиеся комментарии.

```csharp
public ThreadedCommentAuthor this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            
            // Добавьте авторов и продемонстрируйте использование свойства Item
            authors.Add("John Doe", "john.doe@example.com", "JD");
            authors.Add("Jane Smith", "jane.smith@example.com", "JS");
            
            // Получите доступ к автору с помощью свойства Item
            ThreadedCommentAuthor firstAuthor = authors[0];
            Console.WriteLine($"First author: {firstAuthor.Name}, {firstAuthor.UserId}");
            
            // Установите текущего человека, используя свойство Item
            authors.CurrentPerson = authors[1];
            Console.WriteLine($"Current person: {authors.CurrentPerson.Name}");

            // Добавить цепочные комментарии
            CommentCollection comments = workbook.Worksheets[0].Comments;
            comments.AddThreadedComment("A1", "Comment from " + authors[0].Name, authors[0]);
            comments.AddThreadedComment("A1", "Reply from " + authors[1].Name, authors[1]);

            workbook.Save("ThreadedCommentAuthorsDemo.xlsx");
        }
    }
}
```

### См. также

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ThreadedCommentAuthorCollection indexer (2 of 2)

Возвращает человека, который создает ветвящиеся комментарии.

```csharp
public ThreadedCommentAuthor this[string name] { get; }
```

| Параметр | Описание |
| --- | --- |
| name | Имя автора. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            try
            {
                // Доступ к ThreadedCommentAuthorCollection
                ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;

                // Добавьте несколько авторов, чтобы продемонстрировать свойство Item
                authors.Add("John Doe", "john.doe@example.com", "JD");
                authors.Add("Jane Smith", "jane.smith@example.com", "JS");

                // Получите доступ к авторам с помощью свойства Item (индексатор)
                ThreadedCommentAuthor firstAuthor = authors[0];
                ThreadedCommentAuthor secondAuthor = authors[1];

                // Отобразите информацию об авторе, полученную через свойство Item
                Console.WriteLine($"First author: {firstAuthor.Name}, {firstAuthor.UserId}");
                Console.WriteLine($"Second author: {secondAuthor.Name}, {secondAuthor.UserId}");

                // Установите текущего человека, используя одного из авторов, полученных через свойство Item
                authors.CurrentPerson = authors[0];
                Console.WriteLine($"Current person set to: {authors.CurrentPerson.Name}");

                // Сохраните книгу
                workbook.Save("ThreadedCommentAuthorsItemDemo.xlsx");
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
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


