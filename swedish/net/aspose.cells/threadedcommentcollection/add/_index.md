---
title: "ThreadedCommentCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreadedCommentCollection-metod. Lägger till en trådad kommentar"
type: docs
url: /sv/net/aspose.cells/threadedcommentcollection/add/
---
## ThreadedCommentCollection.Add method

Lägger till en trådad kommentar.

```csharp
public int Add(string text, ThreadedCommentAuthor author)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | String | Texten för den trådade kommentaren. |
| författare | ThreadedCommentAuthor | Författaren till den trådade kommentaren |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadedCommentCollectionMethodAddWithStringThreadedCommentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data för sammanhang
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Skapa en trådad kommentarförfattare med hjälp av ThreadedCommentAuthorCollection
                ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
                int authorIndex = authors.Add("John Doe", "john.doe@example.com", "EXAMPLE_PROVIDER");
                ThreadedCommentAuthor author = authors[authorIndex];

                // Åtkomst till den trådade kommentarsamlingen för en cell
                Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
                ThreadedCommentCollection threadedComments = comment.ThreadedComments;

                // Anropa Add‑metoden med String och ThreadedCommentAuthor‑parametrar
                int commentIndex = threadedComments.Add("This is a threaded comment", author);

                // Visa resultatet
                Console.WriteLine($"Added threaded comment at index: {commentIndex}");
                Console.WriteLine($"Comment text: {threadedComments[commentIndex].Notes}");
                Console.WriteLine($"Author: {threadedComments[commentIndex].Author.Name}");

                // Spara arbetsboken
                workbook.Save("ThreadedCommentAddDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


