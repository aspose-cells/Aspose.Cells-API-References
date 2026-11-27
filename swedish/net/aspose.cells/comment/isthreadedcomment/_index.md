---
title: "Comment.IsThreadedComment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Comment-egenskap. Anger om denna kommentar är en trådad kommentar"
type: docs
url: /sv/net/aspose.cells/comment/isthreadedcomment/
---
## Comment.IsThreadedComment property

Anger om denna kommentar är en trådad kommentar.

```csharp
public bool IsThreadedComment { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyIsThreadedCommentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en vanlig kommentar
            Comment regularComment = worksheet.Comments[worksheet.Comments.Add("A1")];
            regularComment.Note = "This is a regular comment";
            regularComment.Author = "User1";

            // Lägg till en trådad kommentar (förutsatt att API:et stödjer att lägga till trådade kommentarer)
            Comment threadedComment = worksheet.Comments[worksheet.Comments.Add("B1")];
            threadedComment.Note = "This is a threaded comment";
            threadedComment.Author = "User2";

            // Kontrollera kommentarstyper
            Console.WriteLine("Comment at A1 is threaded: " + regularComment.IsThreadedComment);
            Console.WriteLine("Comment at B1 is threaded: " + threadedComment.IsThreadedComment);

            // Bearbeta kommentarer baserat på deras typ
            foreach (Comment comment in worksheet.Comments)
            {
                if (comment.IsThreadedComment)
                {
                    Console.WriteLine($"Threaded comment found at {CellsHelper.CellIndexToName(comment.Row, comment.Column)}");
                    Console.WriteLine($"Author: {comment.Author}, Note: {comment.Note}");
                }
                else
                {
                    Console.WriteLine($"Regular comment found at {CellsHelper.CellIndexToName(comment.Row, comment.Column)}");
                }
            }
        }
    }
}
```

### Se även

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


