---
title: "ThreadedCommentAuthorCollection.CurrentPerson"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ThreadedCommentAuthorCollection proprietà. Restituisce e imposta l'utente corrente"
type: docs
url: /it/net/aspose.cells/threadedcommentauthorcollection/currentperson/
---
## ThreadedCommentAuthorCollection.CurrentPerson property

Ottiene e imposta l'utente corrente.

```csharp
public ThreadedCommentAuthor CurrentPerson { get; set; }
```

### Esempi

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

### Vedi anche

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


