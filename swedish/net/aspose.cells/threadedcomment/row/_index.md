---
title: "ThreadedComment.Row"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreadedComment property. Hämtar radindexet för kommentaren"
type: docs
url: /sv/net/aspose.cells/threadedcomment/row/
---
## ThreadedComment.Row property

Hämtar radindexet för kommentaren.

```csharp
public int Row { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Skapa en författare för en trådad kommentar
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                author.Name = "Test Author";
                author.UserId = "test@example.com";
                
                // Lägg till en trådad kommentar i cell B2 (rad 1, kolumn 1)
                worksheet.Comments.AddThreadedComment(1, 1, "Sample threaded comment", author);
                
                // Hämta den första trådade kommentaren
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];
                
                // Visa värdet för egenskapen Row (skrivskyddad)
                Console.WriteLine("Threaded comment row index: " + comment.Row);
                
                // Verifiera att radindexet matchar där vi placerade kommentaren
                if (comment.Row == 1)
                {
                    Console.WriteLine("Comment is correctly placed in row 1");
                }
                
                // Spara arbetsboken
                workbook.Save("ThreadedCommentRowDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


