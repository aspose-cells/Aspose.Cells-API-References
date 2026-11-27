---
title: "Klass ThreadedComment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ThreadedComment-klass. Representerar den trådade kommentaren"
type: docs
url: /sv/net/aspose.cells/threadedcomment/
---
## ThreadedComment class

Representerar den trådade kommentaren.

```csharp
public class ThreadedComment
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Author](../../aspose.cells/threadedcomment/author/) { get; set; } | Hämtar författaren till kommentaren. |
| [Column](../../aspose.cells/threadedcomment/column/) { get; } | Hämtar kolumnindexet för kommentaren. |
| [CreatedTime](../../aspose.cells/threadedcomment/createdtime/) { get; set; } | Hämtar och anger skapandetiden för denna trådade kommentar. |
| [Notes](../../aspose.cells/threadedcomment/notes/) { get; set; } | Hämtar och anger texten för kommentaren. |
| [Row](../../aspose.cells/threadedcomment/row/) { get; } | Hämtar radindexet för kommentaren. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassThreadedCommentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till författare i arbetsboken
            int author1Id = workbook.Worksheets.ThreadedCommentAuthors.Add("User1", "user1@example.com", "1");
            int author2Id = workbook.Worksheets.ThreadedCommentAuthors.Add("User2", "", "2");
            
            // Hämta författarreferenser
            ThreadedCommentAuthor author1 = workbook.Worksheets.ThreadedCommentAuthors[author1Id];
            ThreadedCommentAuthor author2 = workbook.Worksheets.ThreadedCommentAuthors[author2Id];
            
            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Lägg till trådad kommentar till kommentaren
            int threadedCommentIndex = comment.ThreadedComments.Add("This is a threaded comment", author1);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Ange ytterligare egenskaper
            threadedComment.Notes = "Additional notes";
            
            // Lägg till ett svar på den trådade kommentaren
            int replyIndex = comment.ThreadedComments.Add("This is a reply", author2);
            ThreadedComment reply = comment.ThreadedComments[replyIndex];
            
            // Spara arbetsboken
            workbook.Save("ThreadedCommentDemo.xlsx");
            
            Console.WriteLine("Threaded comment demo completed.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


