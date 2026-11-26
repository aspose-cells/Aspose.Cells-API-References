---
title: "ThreadedCommentAuthorCollection.CurrentPerson"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreadedCommentAuthorCollection. Получает и задает текущего пользователя"
type: docs
url: /ru/net/aspose.cells/threadedcommentauthorcollection/currentperson/
---
## ThreadedCommentAuthorCollection.CurrentPerson property

Получает и задает текущего пользователя.

```csharp
public ThreadedCommentAuthor CurrentPerson { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorCollectionPropertyCurrentPersonDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            int authorIndex = authors.Add("Jane Smith", "jane.smith@example.com", "provider456");
            ThreadedCommentAuthor author = authors[authorIndex];

            authors.CurrentPerson = author;
            Console.WriteLine("Current Person: " + authors.CurrentPerson.Name);

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


