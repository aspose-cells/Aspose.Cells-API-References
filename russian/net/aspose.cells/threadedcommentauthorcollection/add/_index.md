---
title: "ThreadedCommentAuthorCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ThreadedCommentAuthorCollection. Добавляет одного автора комментария в ветке"
type: docs
url: /ru/net/aspose.cells/threadedcommentauthorcollection/add/
---
## ThreadedCommentAuthorCollection.Add method

Добавляет одного участника цепочечного комментария.

```csharp
public int Add(string name, string userId, string providerId)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя человека. |
| userId | String |  |
| providerId | String | Идентификатор поставщика |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorCollectionMethodAddWithStringStringStringDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить автора вложенного комментария
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Test Author", "testuser", "TA");

            // Получить добавленного автора
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // Добавить ветвящиеся комментарии с использованием автора
            worksheet.Comments.AddThreadedComment("C2", "First comment", author);
            worksheet.Comments.AddThreadedComment("C2", "Second comment", author);

            // Сохраните книгу
            workbook.Save("ThreadedCommentsExample.xlsx");
        }
    }
}
```

### См. также

* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


