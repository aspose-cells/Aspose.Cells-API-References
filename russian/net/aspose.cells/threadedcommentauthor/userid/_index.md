---
title: "ThreadedCommentAuthor.UserId"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreadedCommentAuthor. Получает и задает идентификатор пользователя"
type: docs
url: /ru/net/aspose.cells/threadedcommentauthor/userid/
---
## ThreadedCommentAuthor.UserId property

Получает и задает идентификатор пользователя.

```csharp
public string UserId { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorPropertyUserIdDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавьте автора вложенного комментария с именем, userId и providerId
                int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD123", "PROVIDER123");

                // Получите объект ThreadedCommentAuthor
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

                // Отобразите значение UserId (операция чтения)
                Console.WriteLine("Author UserId: " + author.UserId);

                // Продемонстрируйте установку нового UserId (операция записи)
                author.UserId = "NEW_USER_ID";
                Console.WriteLine("Updated UserId: " + author.UserId);

                // Создайте вложенный комментарий, используя автора
                worksheet.Comments.AddThreadedComment("A1", "This is a sample comment", author);

                // Сохраните книгу
                workbook.Save("UserIdDemo.xlsx");

                Console.WriteLine("UserId property demonstration completed successfully.");
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

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


