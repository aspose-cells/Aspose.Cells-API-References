---
title: "ThreadedComment.Author"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreadedComment-egenskap. Hämtar författaren till kommentaren"
type: docs
url: /sv/net/aspose.cells/threadedcomment/author/
---
## ThreadedComment.Author property

Hämtar författaren till kommentaren.

```csharp
public ThreadedCommentAuthor Author { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentPropertyAuthorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Hämta standardförfattaren för trådade kommentarer från arbetsboken
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[0];
                author.Name = "John Doe";
                author.UserId = "john.doe@example.com";

                // Lägg till en trådad kommentar i cell A1 (rad 0, kolumn 0)
                worksheet.Comments.AddThreadedComment(0, 0, "Sample comment", author);

                // Hämta den första trådade kommentaren
                ThreadedComment comment = worksheet.Comments[0].ThreadedComments[0];

                // Visa värdet för egenskapen Author (läsoperation)
                Console.WriteLine("Author Name: " + comment.Author.Name);
                Console.WriteLine("Author UserId: " + comment.Author.UserId);
                Console.WriteLine("Author ProviderId: " + comment.Author.ProviderId);

                // Demonstrera att sätta egenskapen Author (eftersom den är läs/skriv)
                ThreadedCommentAuthor newAuthor = workbook.Worksheets.ThreadedCommentAuthors[0];
                newAuthor.Name = "Jane Smith";
                newAuthor.UserId = "jane.smith@example.com";
                comment.Author = newAuthor;

                // Visa det uppdaterade värdet för egenskapen Author
                Console.WriteLine("Updated Author Name: " + comment.Author.Name);
                Console.WriteLine("Updated Author UserId: " + comment.Author.UserId);

                // Spara arbetsboken
                workbook.Save("ThreadedCommentAuthorDemo.xlsx");
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

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


