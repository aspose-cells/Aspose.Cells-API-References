---
title: "ThreadedCommentAuthor.ProviderId"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreadedCommentAuthor-egenskap. Hämtar leverantörens id"
type: docs
url: /sv/net/aspose.cells/threadedcommentauthor/providerid/
---
## ThreadedCommentAuthor.ProviderId property

Hämtar leverantörens id.

```csharp
public string ProviderId { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorPropertyProviderIdDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Lägg till en trådad kommentarsförfattare och hämta dess index
                int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD123", "PROVIDER123");
                
                // Hämta ThreadedCommentAuthor-objektet
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];
                
                // Visa ProviderId-värdet (läsoperation)
                Console.WriteLine("Author ProviderId: " + author.ProviderId);
                
                // Skapa en trådad kommentar med författaren
                worksheet.Comments.AddThreadedComment("A1", "This is a sample comment", author);
                
                // Spara arbetsboken
                workbook.Save("ThreadedCommentAuthorDemo.xlsx");
                
                Console.WriteLine("Demo completed successfully.");
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

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


