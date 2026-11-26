---
title: "WorksheetCollection.ThreadedCommentAuthors"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorksheetCollection. Получает список авторов вложенных комментариев"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/threadedcommentauthors/
---
## WorksheetCollection.ThreadedCommentAuthors property

Получает список авторов ветвящихся комментариев.

```csharp
public ThreadedCommentAuthorCollection ThreadedCommentAuthors { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyThreadedCommentAuthorsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить автора вложенного комментария
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Demo Author", "demo", "DA");

            // Получить автора, которого мы только что добавили
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // Добавить вложенные комментарии в ячейку C2
            AddThreadedComment(worksheet, "C2", "First comment", author);
            AddThreadedComment(worksheet, "C2", "Second comment", author);
            AddThreadedComment(worksheet, "C2", "Third comment", author);

            // Сохраните книгу
            workbook.Save("ThreadedCommentsDemo.xlsx");
        }

        private static void AddThreadedComment(Worksheet worksheet, string cellName, string text, ThreadedCommentAuthor author)
        {
            // Получить ячейку, в которую мы хотим добавить комментарий
            Cell cell = worksheet.Cells[cellName];
            
            // Добавить вложенный комментарий (возвращает void, а не ThreadedComment)
            worksheet.Comments.AddThreadedComment(cellName, text, author);
        }
    }
}
```

### См. также

* class [ThreadedCommentAuthorCollection](../../threadedcommentauthorcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


