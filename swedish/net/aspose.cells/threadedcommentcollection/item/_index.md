---
title: "ThreadedCommentCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreadedCommentCollection‑egenskap. Hämtar den trådade kommentaren med det specifika indexet"
type: docs
url: /sv/net/aspose.cells/threadedcommentcollection/item/
---
## ThreadedCommentCollection indexer

Hämtar den trådade kommentaren med det specifika indexet.

```csharp
public ThreadedComment this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "Initial comment";

            // Lägg till trådade kommentarer
            ThreadedCommentCollection threadedComments = comment.ThreadedComments;
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            
            // Lägg till författare
            int author1Index = authors.Add("User1", "user1@example.com", "ID1");
            int author2Index = authors.Add("User2", "user2@example.com", "ID2");

            // Lägg till trådade kommentarer
            threadedComments.Add("Reply 1", authors[author1Index]);
            threadedComments.Add("Reply 2", authors[author2Index]);

            // Demonstrera användning av Item-egenskapen
            ThreadedComment firstComment = threadedComments[0];
            ThreadedComment secondComment = threadedComments[1];

            Console.WriteLine("First comment author: " + firstComment.Author.Name);
            Console.WriteLine("Second comment author: " + secondComment.Author.Name);

            // Ändra den andra kommentarens författare
            secondComment.Author = authors[author1Index];
            Console.WriteLine("Updated second comment author: " + secondComment.Author.Name);

            // Spara arbetsboken
            workbook.Save("ThreadedCommentsDemo.xlsx");
        }
    }
}
```

### Se även

* class [ThreadedComment](../../threadedcomment/)
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


