---
title: "ThreadedCommentCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreadedCommentCollection-Eigenschaft. Gibt den Threaded-Kommentar anhand des angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells/threadedcommentcollection/item/
---
## ThreadedCommentCollection indexer

Ruft den Threaded-Kommentar am angegebenen Index ab.

```csharp
public ThreadedComment this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der Index |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kommentar hinzufügen
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "Initial comment";

            // Threaded-Kommentare hinzufügen
            ThreadedCommentCollection threadedComments = comment.ThreadedComments;
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            
            // Autoren hinzufügen
            int author1Index = authors.Add("User1", "user1@example.com", "ID1");
            int author2Index = authors.Add("User2", "user2@example.com", "ID2");

            // Threaded-Kommentare hinzufügen
            threadedComments.Add("Reply 1", authors[author1Index]);
            threadedComments.Add("Reply 2", authors[author2Index]);

            // Demonstriere die Verwendung der Item-Eigenschaft
            ThreadedComment firstComment = threadedComments[0];
            ThreadedComment secondComment = threadedComments[1];

            Console.WriteLine("First comment author: " + firstComment.Author.Name);
            Console.WriteLine("Second comment author: " + secondComment.Author.Name);

            // Autor des zweiten Kommentars ändern
            secondComment.Author = authors[author1Index];
            Console.WriteLine("Updated second comment author: " + secondComment.Author.Name);

            // Speichere die Arbeitsmappe
            workbook.Save("ThreadedCommentsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ThreadedComment](../../threadedcomment/)
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


