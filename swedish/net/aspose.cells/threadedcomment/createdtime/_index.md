---
title: "ThreadedComment.CreatedTime"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreadedComment property. Hämtar och sätter skapandetiden för denna trådade kommentar"
type: docs
url: /sv/net/aspose.cells/threadedcomment/createdtime/
---
## ThreadedComment.CreatedTime property

Hämtar och anger skapandetiden för denna trådade kommentar.

```csharp
public DateTime CreatedTime { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentPropertyCreatedTimeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en författare för en trådad kommentar
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors["User1"];
            
            // Lägg till en kommentar till cell A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Lägg till en trådad kommentar
            int threadedCommentIndex = comment.ThreadedComments.Add("Test comment", author);
            ThreadedComment threadedComment = comment.ThreadedComments[threadedCommentIndex];
            
            // Demonstrera egenskapen CreatedTime
            Console.WriteLine("Threaded comment created at: " + threadedComment.CreatedTime);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


