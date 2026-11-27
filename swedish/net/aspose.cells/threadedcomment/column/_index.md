---
title: "ThreadedComment.Column"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreadedComment property. Hämtar kolumnindexet för kommentaren"
type: docs
url: /sv/net/aspose.cells/threadedcomment/column/
---
## ThreadedComment.Column property

Hämtar kolumnindexet för kommentaren.

```csharp
public int Column { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Skapa först en författare för en trådad kommentar
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                
                // Lägg till en trådad kommentar i cell A1 (rad 0, kolumn 0)
                int commentRow = 0;
                int commentColumn = 0;
                worksheet.Comments.AddThreadedComment(commentRow, commentColumn, "Sample comment text", author);
                
                // Hämta den första trådade kommentaren
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];
                
                // Visa värdet för egenskapen Column (skrivskyddad)
                Console.WriteLine("Threaded comment column index: " + comment.Column);
                
                // Verifiera att kolumnindexet matchar där vi placerade kommentaren
                if (comment.Column == commentColumn)
                {
                    Console.WriteLine("Comment is correctly placed in column " + commentColumn);
                }
                
                // Spara arbetsboken
                workbook.Save("ThreadedCommentColumnDemo.xlsx");
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


