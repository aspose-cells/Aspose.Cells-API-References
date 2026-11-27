---
title: "ThreadedCommentAuthor.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreadedCommentAuthor-egenskap. Hämtar och anger namnet"
type: docs
url: /sv/net/aspose.cells/threadedcommentauthor/name/
---
## ThreadedCommentAuthor.Name property

Hämtar och anger namnet.

```csharp
public string Name { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorPropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en kommentar och trådade kommentarer
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Initial comment";
            ThreadedCommentCollection threadedComments = comment.ThreadedComments;
            
            // Lägg till trådade kommentarer med olika författare
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            int author1Index = authors.Add("User1", "user1@example.com", "ID1");
            int author2Index = authors.Add("User2", "user2@example.com", "ID2");

            // Lägg till trådade kommentarer
            threadedComments.Add("Reply from User1", authors[author1Index]);
            threadedComments.Add("Reply from User2", authors[author2Index]);

            // Demonstrera användning av Name‑egenskapen
            Console.WriteLine("First author name: " + threadedComments[0].Author.Name);
            Console.WriteLine("Second author name: " + threadedComments[1].Author.Name);

            // Ändra författare för den andra kommentaren
            threadedComments[1].Author = authors[author1Index];
            Console.WriteLine("Updated second author name: " + threadedComments[1].Author.Name);

            // Spara arbetsboken
            workbook.Save("ThreadedCommentAuthorsDemo.xlsx");
        }
    }
}
```

### Se även

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


