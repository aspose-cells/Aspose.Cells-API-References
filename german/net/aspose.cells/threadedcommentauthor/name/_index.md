---
title: "ThreadedCommentAuthor.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreadedCommentAuthor-Eigenschaft. Liest und schreibt den Namen"
type: docs
url: /de/net/aspose.cells/threadedcommentauthor/name/
---
## ThreadedCommentAuthor.Name property

Liest und setzt den Namen.

```csharp
public string Name { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorPropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einen Kommentar und ThreadedComments hinzu
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Initial comment";
            ThreadedCommentCollection threadedComments = comment.ThreadedComments;
            
            // Füge ThreadedComments mit verschiedenen Autoren hinzu
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            int author1Index = authors.Add("User1", "user1@example.com", "ID1");
            int author2Index = authors.Add("User2", "user2@example.com", "ID2");

            // Threaded-Kommentare hinzufügen
            threadedComments.Add("Reply from User1", authors[author1Index]);
            threadedComments.Add("Reply from User2", authors[author2Index]);

            // Demonstrieren Sie die Verwendung der Name-Eigenschaft
            Console.WriteLine("First author name: " + threadedComments[0].Author.Name);
            Console.WriteLine("Second author name: " + threadedComments[1].Author.Name);

            // Ändere den Autor des zweiten Kommentars
            threadedComments[1].Author = authors[author1Index];
            Console.WriteLine("Updated second author name: " + threadedComments[1].Author.Name);

            // Speichere die Arbeitsmappe
            workbook.Save("ThreadedCommentAuthorsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


