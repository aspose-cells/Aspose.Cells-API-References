---
title: "ThreadedCommentAuthor.UserId"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreadedCommentAuthor-egenskap. Hämtar och anger användarens id"
type: docs
url: /sv/net/aspose.cells/threadedcommentauthor/userid/
---
## ThreadedCommentAuthor.UserId property

Hämtar och anger användarens id.

```csharp
public string UserId { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentAuthorPropertyUserIdDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till en trådad kommentarsförfattare med namn, userId och providerId
                int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("John Doe", "JD123", "PROVIDER123");

                // Hämta ThreadedCommentAuthor-objektet
                ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

                // Visa UserId-värdet (läsoperation)
                Console.WriteLine("Author UserId: " + author.UserId);

                // Demonstrera att sätta ett nytt UserId (skrivoperation)
                author.UserId = "NEW_USER_ID";
                Console.WriteLine("Updated UserId: " + author.UserId);

                // Skapa en trådad kommentar med författaren
                worksheet.Comments.AddThreadedComment("A1", "This is a sample comment", author);

                // Spara arbetsboken
                workbook.Save("UserIdDemo.xlsx");

                Console.WriteLine("UserId property demonstration completed successfully.");
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


