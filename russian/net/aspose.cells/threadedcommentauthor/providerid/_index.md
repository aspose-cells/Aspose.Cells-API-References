---
title: "ThreadedCommentAuthor.ProviderId"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreadedCommentAuthor. Получает идентификатор поставщика"
type: docs
url: /ru/net/aspose.cells/threadedcommentauthor/providerid/
---
## ThreadedCommentAuthor.ProviderId property

Получает идентификатор поставщика.

```csharp
public string ProviderId { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorPropertyProviderIdDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Добавьте автора вложенного комментария и получите его индекс
                int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD123", "PROVIDER123");
                
                // Получите объект ThreadedCommentAuthor
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
                
                // Отобразите значение ProviderId (операция чтения)
                Console.WriteLine("Author ProviderId: " + author.ProviderId);
                
                // Создайте вложенный комментарий, используя автора
                worksheet.Comments.AddThreadedComment("A1", "This is a sample comment", author);
                
                // Сохраните книгу
                workbook.Save("ThreadedCommentAuthorDemo.xlsx");
                
                Console.WriteLine("Demo completed successfully.");
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


